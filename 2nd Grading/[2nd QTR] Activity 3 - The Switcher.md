![INTERFACE - Act3TSwitcherHumility Follosco](https://user-images.githubusercontent.com/94034753/146489897-544eb667-3c57-4a55-a53e-57130fc4e3c8.png)
<h3>Required Elements:</h3></br>

/tba/
________________________________________________________________________________________________________________________
```
Public Class frmThe_Switcher
    'Programmed by: Name
    'Date: Date

    Private Sub radWhite_CheckedChanged(sender As Object, e As EventArgs) Handles radWhite.CheckedChanged
        lblLight.ForeColor = Color.White
    End Sub

    Private Sub radRed_CheckedChanged(sender As Object, e As EventArgs) Handles radRed.CheckedChanged
        lblLight.ForeColor = Color.Red
    End Sub

    Private Sub radOrange_CheckedChanged(sender As Object, e As EventArgs) Handles radOrange.CheckedChanged
        lblLight.ForeColor = Color.Orange
    End Sub

    Private Sub radYellow_CheckedChanged(sender As Object, e As EventArgs) Handles radYellow.CheckedChanged
        lblLight.ForeColor = Color.Yellow
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
