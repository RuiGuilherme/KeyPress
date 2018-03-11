# KeyPress
Detect key pressed in Textbox WPF
# MainWindow.xaml:

**_<TextBox x:Name="TextBoxExempleName" Text="{Binding Path=TextBoxExempleBinding}" KeyDown="Testkeys" Grid.Row="1" Margin="5" />_**

# MainWindow.xaml.cs:
**_private void Testkeys(object sender, KeyEventArgs e)
{
        //Get x:Name TextBox
        var TextBox = (TextBox)sender;
        //Call KeyPress
        new KeyPress(e);
        //Assigns the values in the textbox
        TextBox.Text = KeyPress.Text;
    }
}_**
