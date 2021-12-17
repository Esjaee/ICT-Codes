![INTERFACE - Act3TSwitcherHumility Follosco](https://user-images.githubusercontent.com/94034753/146489897-544eb667-3c57-4a55-a53e-57130fc4e3c8.png)
<h3>Required Elements:</h3></br>

2 Light Bulb Images <br/>
→ These are the light bulb images to be used in the interface. <br/>
→ In the upper right arrow button of the picture box, press "Choose Image"<br/>
→ Choose "Project Resource File" then click import. Find the light bulb images you saved from the internet then press "OK".

2 Picture Boxes <br/>
→ These is where we will put the light bulb images. <br/>
→ Names: <br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "pboLightsOn" (Lights on img) </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "pboLightsOff" (Lights off img)</br>
→ Required Properties (In upper right button of box): </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ Size Mode: Zoom </br>

2 Regular Labels </br>
→ These are static labels that have no code, no need to change element name, only the text. </br>
→ Text: </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→"Name:"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→"Programmed by: "</br>

1 Blank Label </br>
→ This is where the generated text will appear. </br>
→ Name: "lblLight"</br>
→ Text: "&nbsp;&nbsp;&nbsp;"</br>

1 Blank Textboxes </br>
→ These are blank textboxes where we will input information. </br>
→ Name: </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "txtName"</br>

2 Function Buttons </br>
→ Coded Buttons; When pressed, funtion should occur. </br>
→ Name:</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "btnPrint"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "btnExit"</br>
→ Text: </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "Print"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "Exit"</br>

1 Group Box <br/>
→ This is where you will put the Radio Buttons <br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ Text: "Choose a color" <br/>

4 Radio Buttons <br/>
→ This where the user will choose the color of the blank label (lblLight) <br/>
→ Name: <br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "radColor" <br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ Replace rad"Color with other colors. EX: "radRed", "radBlue", etc. <br/>

Print Button (VB19) <br/>
→ To print your form in VB19, insert "PrintDocument" from toolbox to interface. <br/>
→ Name: "PrintTheSwitcher" <br/>
→ Then, input VB19 Print code from the code below.

<h3>🟥Code Reminders:🟥</h3></br>
→ Do not copy theme in example! </br>
→ Different sections might have different coding/naming requirements. Please follow this.</br>
→ Don't forget to remove the control box from your form. (Window Style > ControlBox: "False")</br>
→ Replace "(Choose Color)" with Colors in VB like "Red", "Blue", etc. <br/>

_________________________________________________________________________________________________

```
Public Class frmThe_Switcher

    Private Sub radColor_CheckedChanged(sender As Object, e As EventArgs) Handles radWhite.CheckedChanged
        lblLight.ForeColor = Color.(Choose Color)
    End Sub

    Private Sub radColor2_CheckedChanged(sender As Object, e As EventArgs) Handles radRed.CheckedChanged
        lblLight.ForeColor = Color.(Choose Color)
    End Sub

    Private Sub radColor3_CheckedChanged(sender As Object, e As EventArgs) Handles radOrange.CheckedChanged
        lblLight.ForeColor = Color.(Choose Color)
    End Sub

    Private Sub radColor4_CheckedChanged(sender As Object, e As EventArgs) Handles radYellow.CheckedChanged
        lblLight.ForeColor = Color.(Choose Color)
    End Sub

    Private Sub pboLightsOff_Click(sender As Object, e As EventArgs) Handles pboLightsOff.Click
        pboLightsOff.Visible = False
        pboLightsOn.Visible = True
        lblLight.Text = "Please turn off the light, " & txtName.Text & ""
    End Sub

    Private Sub pboLightsOn_Click(sender As Object, e As EventArgs) Handles pboLightsOn.Click
        pboLightsOn.Visible = False
        pboLightsOff.Visible = True
        lblLight.Text = "Please turn on the light, " & txtName.Text & ""
    End Sub

    Private Sub btnPrint_Click(sender As Object, e As EventArgs) Handles btnPrint.Click
        'VB19 (Insert PrintDocument in Interface for this to work) : PrintTheSwitcher.Print()
        'VB08 : PrintForm1.PrintAction = Printing.PrintAction.PrintToPreview
                PrintForm1.Print()
    End Sub

    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        Me.Close()
    End Sub
End Class
```
