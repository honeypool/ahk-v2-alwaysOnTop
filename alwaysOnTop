^space:: ;ctrl+space
  {
    active:= WinGetTitle("A")
    If !(WinGetMinMax(active))
	  {
        WinSetAlwaysOnTop -1, active
	    ExStyle := WinGetExStyle(active)
        If ((ExStyle & 0x8))
          ToolTip active "`nis always-on-top now."
	    else
	      ToolTip active "`nis NOT always-on-top anymore."
	  }
    else
      ToolTip "Maximized windows are protected to be always-on-top"
    SetTimer () => ToolTip(), -4000
 }
