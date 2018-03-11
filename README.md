# KeyPress
Detect key pressed in Textbox WPF

## MainWindow.xaml:
```
<TextBox x:Name="TextBoxExempleName" Text="{Binding Path=TextBoxExempleBinding}" KeyDown="Testkeys">
<TextBox x:Name="TextBoxExempleName2" Text="{Binding Path=TextBoxExempleBinding2}" KeyDown="Testkeys">
<TextBox x:Name="TextBoxExempleName3" Text="{Binding Path=TextBoxExempleBinding23" KeyDown="Testkeys">
```
## MainWindow.xaml.cs:
```
using KeyPress;
private void Testkeys(object sender, KeyEventArgs e)
 {
      //Get x:Name TextBox
        var TextBox = (TextBox)sender;
      //Call KeyPress
       new KeyPress(e);
      //Assigns the values in the textbox
       TextBox.Text = KeyPress.Text;
   }
}
```
