# License for Sublime Text build 4143
1. Go to https://hexed.it/
2. Click on the "Open file" button in the top left corner and select sublime_text (located in: /opt/sublime_text/sublime_text)
3. Go back to hexed.it and in the top right corner we will see the search tag, where we will enter the following code: 80 78 05 00 0F 94 C1
4. The code will be highlighted and we must replace it one by one with the following: C6 40 05 01 48 85 C9
5. Click on the "Save as" button and save it to the downloads folder.
6. Open the terminal and write the following commands:

```bash
sudo mv /opt/sublime_text/sublime_text ./sublime_text.old    # Rename old sublime_text to sublime_text.old
cd $HOME/Downloads/    # Enter the Downloads folder
sudo chmod 755 sublime_text    # Give permissions to the "new" sublime_text
sudo chown root sublime_text    # Change the owner of the file to "root"
sudo chgrp root sublime_text    # Change the owner group to "root"
sudo mv sublime_text /opt/sublime_text/    # Move the new sublime_text to the original directory
```

If we reopen Sublime Text we should now have the license.  
To confirm, we should go to the top "Help > About Sublime Text" and the message "Unlimited User Licence" should appear.  
(Note that it should work in more versions, but I have only tested it in 4143.)  
### Done! I hope it helps you.
