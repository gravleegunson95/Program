# Program
Local $Part = 1;The "part" number of the status bar to read - the default is 1. 1 is the first possible part and usually the one that contains the useful messages like "Ready" "Loading...", etc. While 1 Local $sText = StatusbarGetText("title of window here",'',$Part) Local $word = "Finished" if StringInStr($sText,$word) Then WinClose("Program - ","") ExitLoop Endif Sleep(50) Wend
