![Output](https://user-images.githubusercontent.com/94034753/144513316-af409350-e512-4cec-9de7-09f74fdd6099.jpg)

<h3>Required Elements:</h3></br>

5 blank text boxes </br>
  → In this example, it's named txt1N. Please change it when copying the code. </br>

7 Buttons </br>
  → Clear Button and Exit Button </br>
  → Sum, Diff, Prod, Quotient buttons. (Name: btnSum, btnDifference, etc.) </br>

5 labels </br>
  → Labels where the computed number will appear. (Name: lblSum, lblDifference, etc.) </br>
________________________________________________________________________________________________________________________
```
Public Class frmVariable
    Dim First_No, Second_No, Third_No, Fourth_No, Fifth_No As Double

    Dim Sum As Double
    Private Sub btnSum_Click(sender As Object, e As EventArgs) Handles btnSum.Click
        First_No = txt1N.Text
        Second_No = txt2N.Text
        Third_No = txt3N.Text
        Fourth_No = txt4N.Text
        Fifth_No = txt5N.Text
        Sum = First_No + Second_No + Third_No + Fourth_No + Fifth_No
        lblSum.Text = Sum
    End Sub

    Dim Difference As Double
    Private Sub btnDifference_Click(sender As Object, e As EventArgs) Handles btnDifference.Click
        First_No = txt1N.Text
        Second_No = txt2N.Text
        Third_No = txt3N.Text
        Fourth_No = txt4N.Text
        Fifth_No = txt5N.Text
        Difference = First_No - Second_No - Third_No - Fourth_No - Fifth_No
        lblDifference.Text = Difference
    End Sub

    Dim Product As Double
    Private Sub btnProduct_Click(sender As Object, e As EventArgs) Handles btnProduct.Click
        First_No = txt1N.Text
        Second_No = txt2N.Text
        Third_No = txt3N.Text
        Fourth_No = txt4N.Text
        Fifth_No = txt5N.Text
        Product = First_No * Second_No * Third_No * Fourth_No * Fifth_No
        lblProduct.Text = Product
    End Sub

    Dim Quotient As Double
    Private Sub btnQuotient_Click(sender As Object, e As EventArgs) Handles btnQuotient.Click
        First_No = txt1N.Text
        Second_No = txt2N.Text
        Third_No = txt3N.Text
        Fourth_No = txt4N.Text
        Fifth_No = txt5N.Text
        Quotient = First_No / Second_No / Third_No / Fourth_No / Fifth_No
        lblQuotient.Text = Quotient
    End Sub

    Private Sub btnClear_Click(sender As Object, e As EventArgs) Handles btnClear.Click
        txt1N.Clear()
        txt2N.Clear()
        txt3N.Clear()
        txt4N.Clear()
        txt5N.Clear()
    End Sub

    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        Me.Close()
    End Sub
End Class
```
