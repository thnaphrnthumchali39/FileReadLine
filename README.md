# FileReadLine
al $coin[3] If FileExists( "runnumber.txt" ) then Local $sTimesRan = FileReadLine( "runnumber.txt", 1 ) Else Local $sTimesRan = 0 EndIf $coin[1] = "Heads" $Coin[2] = "Tails" While 1    $sTimesRan = $sTimesRan + 1    FileDelete( "runnumber.txt" )    FileWrite ( "runnumber.txt", $sTimesRan ) MsgBox(0, "Coin Flip" &amp; " - " &amp; $sTimesRan , $Coin[Random(1, 2, 1)]) WEnd
