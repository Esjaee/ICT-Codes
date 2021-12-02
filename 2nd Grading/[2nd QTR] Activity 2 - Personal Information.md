![Activity 2 - Personal Information  Follosco](https://user-images.githubusercontent.com/94034753/144510200-4ca41446-7fce-4007-9332-81d0fe1edc22.png)
<h3>Required Elements:</h3></br>

5 Regular Labels </br>
→ These are static labels that have no code, no need to change element name, only the text. </br>
→ Text: </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→"First Name: "</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→"Middle Name: "</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→"Last Name: "</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→"Grade Level: "</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→"Section: "</br>

1 Blank Label </br>
→ This is where the generated text will appear. </br>
→ Name: "lblPersonalInfo"</br>
→ Text: "&nbsp;&nbsp;&nbsp;"</br>
→ Required Properties: </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ Border Style: FixedSingle </br>

5 Blank Textboxes </br>
→ These are blank textboxes where we will input information. </br>
→ Name: </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "txtFName"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "txtMName"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "txtLName"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "txtGradeLevel"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "txtSection"</br>

4 Function Buttons </br>
→ Coded Buttons; When pressed, funtion should occur. </br>
→ Name:</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "btnOk"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "btnClear"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "btnPrint"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "btnExit"</br>
→ Text: </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "Ok"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "Clear"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "Print"</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→ "Exit"</br>

<h3>🟥Code Reminders:🟥</h3></br>
→ Do not copy theme in example! </br>
→ Different sections might have different coding/naming requirements. Please follow this.</br>
→ Print code differs between programs. I am unable to provide the code for VB2008.</br>
________________________________________________________________________________________________________________________
```
Public Class frmPersonalInfo
    Dim FN, MN, LN, GL, Section As String

    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        Me.Close()
    End Sub

    Private Sub btnClear_Click(sender As Object, e As EventArgs) Handles btnClear.Click
        txtFName.Clear()
        txtMName.Clear()
        txtLName.Clear()
        txtGradeLevel.Clear()
        txtSection.Clear()
    End Sub

    Private Sub btnOk_Click(sender As Object, e As EventArgs) Handles btnOk.Click
        FN = txtFName.Text
        MN = txtMName.Text
        LN = txtLName.Text
        GL = txtGradeLevel.Text
        Section = txtSection.Text

        lblPersonalInfo.Text = "Your complete name is " & FN & " " & MN & " " & LN & " and you are in  " & GL & "-" & Section & ". "
    End Sub End Class
