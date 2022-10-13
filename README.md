## Media keys shortcuts for AHK/AutoHotkey

- ctrl + left:   **Next**
- ctrl + right:  **Previous**
- ctrl + up:     **Volume up**
- ctrl + down:   **Volume down**
- ctrl + space:  **Play/Pause**

#### Other shortcuts:
- ^ for ctrl
- ! for alt
- ^ for shift

For full list of keys: https://www.autohotkey.com/docs/Hotkeys.htm

 <hr />

```#NoEnv  ; Recommended for performance and compatibility with future AutoHotkey releases.
; #Warn  ; Enable warnings to assist with detecting common errors.
SendMode Input  ; Recommended for new scripts due to its superior speed and reliability.
SetWorkingDir %A_ScriptDir%  ; Ensures a consistent starting directory.

;Keyboard shortcuts for media keys

^Left::Send	{Media_Prev}
^Right::Send	{Media_Next}
^Up::Send	{Volume_Up}
^Down::Send	{Volume_Down}
^Space::Send	{Media_Play_Pause}```
