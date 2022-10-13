## Media keys shortcuts for AHK/AutoHotkey

- <kbd>ctrl</kbd> + <kbd>left</kbd> : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Next**
- <kbd>ctrl</kbd> + <kbd>right</kbd> : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Previous**
- <kbd>ctrl</kbd> + <kbd>up</kbd> : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Volume up**
- <kbd>ctrl</kbd> + <kbd>down</kbd> : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Volume down**
- <kbd>ctrl</kbd> + <kbd>space</kbd> : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Play/Pause**

#### Other shortcuts:
- ^ for <kbd>ctrl</kbd>
- ! for <kbd>alt</kbd>
- + for <kbd>shift</kbd>

#### Examples
```
Left::Send {Media_Prev

; Previous song by pressing left arrow key
```

```
!^Left::Send	{Media_Prev} 

; Next song by pressing alt + ctrl + left key
```

For full list of keys: https://www.autohotkey.com/docs/Hotkeys.htm

### To get it working on startup
1. <kbd>windows</kbd> + <kbd>r</kbd> (or open up Run)
2. shell:startup
3. Move .ahk file into folder

 <hr />

### My script
```
#NoEnv  ; Recommended for performance and compatibility with future AutoHotkey releases.
; #Warn  ; Enable warnings to assist with detecting common errors.
SendMode Input  ; Recommended for new scripts due to its superior speed and reliability.
SetWorkingDir %A_ScriptDir%  ; Ensures a consistent starting directory.

;Keyboard shortcuts for media keys

^Left::Send	{Media_Prev}
^Right::Send	{Media_Next}
^Up::Send	{Volume_Up}
^Down::Send	{Volume_Down}
^Space::Send	{Media_Play_Pause}
```
