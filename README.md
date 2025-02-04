# project-rs
```vbnet
' これは VB.NET のコードです




Public Class Form1
    ' フォームのロード時にDateTimePickerを初期化
    Private Sub Form1_Load(sender As Object, e As EventArgs) Handles MyBase.Load
        InitializeDateTimePicker()
    End Sub

    ' DateTimePickerの初期化（空白にする）
    Private Sub InitializeDateTimePicker()
        DateTimePicker1.Format = DateTimePickerFormat.Custom
        DateTimePicker1.CustomFormat = "" ' 初期状態を空白に
        DateTimePicker1.ShowCheckBox = False ' チェックボックスを非表示
    End Sub

    ' ユーザーが入力しようとしたら通常の日付フォーマットを適用
    Private Sub DateTimePicker1_Enter(sender As Object, e As EventArgs) Handles DateTimePicker1.Enter
        If DateTimePicker1.CustomFormat = "" Then
            DateTimePicker1.CustomFormat = "yyyy/MM/dd" ' 編集可能にする
            DateTimePicker1.Value = DateTime.Now ' 現在の日付をセット
        End If
    End Sub

    ' Deleteキーで日付を削除
    Private Sub DateTimePicker1_KeyDown(sender As Object, e As KeyEventArgs) Handles DateTimePicker1.KeyDown
        If e.KeyCode = Keys.Delete Then
            InitializeDateTimePicker() ' 初期状態に戻す
            e.SuppressKeyPress = True ' 不要な動作を防ぐ
        End If
    End Sub
End Class
```
