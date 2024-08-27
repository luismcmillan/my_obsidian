[[VBA]]
```
Dim Tag As String
Tag = "Montag"
Select Case Tag
    Case "Montag"
        MsgBox "Es ist Montag"
    Case "Dienstag"
        MsgBox "Es ist Dienstag"
    Case Else
        MsgBox "Es ist ein anderer Tag"
End Select
```