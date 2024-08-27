[[VBA]]
[[Shell]]
```Shell
Shell(PathName As String, [WindowStyle As VbAppWinStyle]) As Double

Sub ÖffneNotepad()
    Shell "notepad.exe", vbNormalFocus
End Sub

Sub AusführenCmdBefehl()
    Shell "cmd.exe /c echo Hallo, Welt! > C:\Pfad\Zu\Datei.txt", vbHide
End Sub

Sub StarteBatchDatei()
    Shell "C:\Pfad\Zu\DeinerBatchDatei.bat", vbNormalFocus
End Sub

#Einfache Datei öffnen
Sub ÖffneTextdatei()
    Shell "notepad.exe C:\Pfad\Zu\DeinerDatei.txt", vbNormalFocus
End Sub

```