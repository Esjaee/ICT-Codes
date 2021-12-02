![Project 1 Output](https://user-images.githubusercontent.com/94034753/144507906-c3c7893b-47ef-4777-bc6b-307106a83341.png)</br>
<h3>Required Elements:</h3></br>

4 Regular Labels </br>
→ These are static labels that have no code, no need to change element name, only the text. </br>
→ Text: "Clothing Store Name" | "Full Name" | "Address:" | "Store Hours:".</br>

2 Blank Labels </br>
→ Blank label where the Aisle Number will appear. </br>
→ Name: "lblAddress" | "lblHours" </br>
→ Text: "&nbsp;&nbsp;&nbsp;" </br>

4 Location Buttons </br>
→ Coded buttons; when pressed, Address should appear on "lblAddress" label. </br>
→ Name: "btnBGC" | "btnMOA" | "btnFestival" | "btnGlorietta" </br>
→ Text: "Uptown Mall-BGC" | "SM Mall of Asia" | "Festival Alabang" | "Glorietta" </br>

2 Function Buttons </br>
→ Coded Buttons; When pressed, funtion should occur. </br>
→ Name: "btnPrint" | "btnExit"
→ Text: "Print" | "Exit"

Code Reminders: </br>
→ Change "Location" with ADDRESS of the store. </br>
→ Change "Time" with Store Hours. </br>
________________________________________________________________________________________________________________________
```
Public Class frmClothingLine
    Private Sub btnBGC_Click(sender As Object, e As EventArgs) Handles btnBGC.Click
        lblAddress.Text = "Location"
        lblHours.Text = "Time"
    End Sub

    Private Sub btnMOA_Click(sender As Object, e As EventArgs) Handles btnMOA.Click
        lblAddress.Text = "Location"
        lblHours.Text = "Time"
    End Sub

    Private Sub btnFestival_Click(sender As Object, e As EventArgs) Handles btnFestival.Click
        lblAddress.Text = "Location"
        lblHours.Text = "Time"
    End Sub

    Private Sub btnGlorietta_Click(sender As Object, e As EventArgs) Handles btnGlorietta.Click
        lblAddress.Text = "Location"
        lblHours.Text = "Time"
    End Sub

    Private Sub btnPrint_Click(sender As Object, e As EventArgs) Handles btnPrint.Click
        Close()
    End Sub

    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        Close()
    End Sub
End Class
```
