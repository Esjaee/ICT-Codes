![Astro Video](https://user-images.githubusercontent.com/94034753/144505696-263125a3-dbf8-45b1-8f7e-d01b0b8a9d41.png)
<h3>Required Elements</hr></br>

3 Regular Labels </br>
→ These are static labels that have no code, no need to change element name, only the text</br>
→ Text: "Location", "Genres", "Name". </br>

1 Blank Label </br>
→ Blank label where the Aisle Number will appear. </br>
→ Name: "lblLocation"</br>
→ Text: "    "</br>

6 Aisle Buttons</br>
→ Coded buttons; when pressed Aisle Number should appear on "lblLocation" label.</br>
→ Name: "btnGenre" (ex: "btnComedy", "btnHorror", etc.)</br>
→ Text: "Genre" (ex: "Comedy", "Horror", etc.)</br>
________________________________________________________________________________________________________________________
```
Public Class frmAstroVideo

	Private Sub btnComedy_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) Handles btnComedy.Click
		lblLocation.Text = “Aisle 1”
	End Sub

	Private Sub btnDrama_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) Handles btnDrama.Click
		lblLocation.Text = “Aisle 2”
	End Sub

	Private Sub btnAction_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) Handles btnAction.Click
		lblLocation.Text = “Aisle 3”
	End Sub

	Private Sub btnScifi_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) Handles btnScifi.Click
		lblLocation.Text = “Aisle 4”
	End Sub

	Private Sub btnHorror_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) Handles btnHorror.Click
		lblLocation.Text = “Aisle 5”
	End Sub

	Private Sub btnNewReleases_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) Handles btnNewReleases.Click
		lblLocation.Text = “Back Wall”
	End Sub

	Private Sub btnPrint_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) Handles btnPrint.Click
		Close ()
	End Sub

	Private Sub btnExit_Click (ByVal sender As System.Object, ByVal e As System.EventArgs) btnExit.Click
		Close ()
	End Sub

End class
```
