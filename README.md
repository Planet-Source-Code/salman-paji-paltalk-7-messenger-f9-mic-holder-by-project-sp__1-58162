<div align="center">

## PalTalk 7 Messenger F9 Mic Holder By Project SP


</div>

### Description

This Will Hold F9 Button To Hold Mic In PalTalk 7 Messenger Rooms, In This I Used F9 Button To Grab Mic, & This Example Can Also Be Used For Other Programz.... As You Can See No Handles Were Used In It...... Have Fun!!.... Use It As You Guyz Like To.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Salman Paji](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/salman-paji.md)
**Level**          |Beginner
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |VB 6\.0
**Category**       |[Windows API Call/ Explanation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows-api-call-explanation__1-39.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/salman-paji-paltalk-7-messenger-f9-mic-holder-by-project-sp__1-58162/archive/master.zip)

### API Declarations

```
Private Declare Sub keybd_event Lib "user32" (ByVal bVk As Byte, ByVal bScan As Byte, ByVal dwFlags As Long, ByVal dwExtraInfo As Long)
Private Const KEYEVENTF_KEYUP = &H2
Private Const VK_F9 = &H78
```


### Source Code

```
'Use Two Buttons.... and Name Them
'"Hold" For Holding Mic on PalTalk
'"Release" For Releasing Mic From Holding On PalTalk
Private Sub Hold_Click()
'Call keybd_event(vbKeyF9, 0, 0, 0)
Call keybd_event(VK_F9, 0, 0, 0)
End Sub
Private Sub Release_Click()
'Call keybd_event(vbKeyF9, 0, vbKeyUp, 0)
Call keybd_event(VK_F9, 0, KEYEVENTF_KEYUP, 0)
End Sub
```

