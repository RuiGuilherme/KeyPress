# KeyPress
Detect key pressed in Textbox WPF
# MainWindow.xaml:
<br />
**_<TextBox x:Name="TextBoxExempleName" Text="{Binding Path=TextBoxExempleBinding}" KeyDown="Testkeys" Grid.Row="1" Margin="5">_**
<br />
# MainWindow.xaml.cs:
<br />
**_private void Testkeys(object sender, KeyEventArgs e)
{
<br />
        //Get x:Name TextBox
        <br />
        var TextBox = (TextBox)sender;
        <br />
        //Call KeyPress
        <br />
        new KeyPress(e);
        <br />
        //Assigns the values in the textbox
        <br />
        TextBox.Text = KeyPress.Text;
        <br />
    }
    <br />
}_**
