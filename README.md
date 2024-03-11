# SeestarS50Organizer
A fast method of organizing Seestar S50 subs. 

1. Open your PowerShell profile for editing. If you're not sure where your profile is located, you can find it by typing $PROFILE in a PowerShell window. The file is usually located at C:\Users\<YourUsername>\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1
2. Using your favorite text editor, add the function to your PowerShell profile
3. Save and close your PowerShell profile
4. Restart PowerShell or reload your profile by executing . $PROFILE

Now, you can use the Organize-Files function in any directory to organize your files as described. Just navigate to the desired folder and run Organize-Files.

If you want to undo the organization quickly:
  Get-ChildItem -Path .\fits,.\jpg,.\thn -File | Move-Item -Destination .
The undo will need to be run in PS within the folder you want to undo the moves. This should work in any folder that has the three folders. (fits, jpg, and thn)
