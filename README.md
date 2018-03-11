# KeyPress
Detect key pressed in Textbox WPF
# MainWindow.xaml:
1. <TextBox x:Name="TextBoxExempleName" Text="{Binding Path=TextBoxExempleBinding}" KeyDown="Testkeys" Grid.Row="1" Margin="5" />

# MainWindow.xaml.cs:
1. private void Testkeys(object sender, KeyEventArgs e)
1. {
1.         //Get x:Name TextBox
1.         var TextBox = (TextBox)sender;
1.         //Call KeyPress
1.         new KeyPress(e);
1.         //Assigns the values in the textbox
1.         TextBox.Text = KeyPress.Text;
1.     }
1. }

