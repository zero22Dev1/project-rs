# project-rs
```vbnet
' これは VB.NET のコードです
' 現在の日付の "yyyy/MM" 形式の文字列
Dim dateString As String = DateTime.Now.ToString("yyyy/MM")

' 文字列を Date 型に変換（1日を仮でセット）
Dim parsedDate As Date = DateTime.ParseExact(dateString & "/01", "yyyy/MM/dd", Nothing)

' C1DateTimePicker の設定
With C1DateTimePicker1
    .Value = parsedDate         ' 値をセット
    .FormatType = C1.Win.C1Input.FormatTypeEnum.CustomFormat ' カスタムフォーマットを使用
    .CustomFormat = "yyyy/MM"   ' "yyyy/MM" 形式で表示
End With