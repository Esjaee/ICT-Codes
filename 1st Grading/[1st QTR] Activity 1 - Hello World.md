![Act1HelloWorld](https://user-images.githubusercontent.com/94034753/144505340-9c88d704-65e4-4480-9027-a83d20db6327.png)
<h3>Required Elements:</h3> </br>

1 Button</br>
→ Name: "btnEnglish"</br>
→ Text: "English"</br>

1 Label</br>
→ Name: "lblMessage"</br>
→ Text: " "</br>
________________________________________________________________________________________________________________________
```
Public Class frmHelloWorld
  Private Sub btnEnglish_Click(sender As Object, e As EventArgs) Handles btnEnglish.Click
    lblMessage.Text = "Hello World"
  End Sub
End Class
```
