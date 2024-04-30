# crossover-unlimited
**This method only works for CrossOver 21. In order for this to work, make sure you have installed CrossOver 21.**

1. Ensure you have installed CrossOver 21 and the Prefs Editor application.
2. Launch Prefs Editor and search for 'CrossOver' in the list. Locate `com.codeweavers.CrossOver` and open it.
3. Navigate to `FirstRunDate` and change the year to 9999. Save the changes and close Prefs Editor.
4. Open CrossOver. Initially, you may encounter an error message stating: "CrossOver is unable to initialize a critical component. Failed to run Python script '/Applications/CrossOver.app/Contents/Resources/libcxsetupbase.py'. See console for errors. The program will now exit."

To resolve this:

4. Open Finder and navigate to your applications folder.
5. Right click on `CrossOver.app`, choose 'Show Package Contents' -> 'Contents' -> 'Resources'.
6. Locate and open the file `libcxsetupbase.py` with a text editor.
7. Change line 6 from `from Foundation import *` to `from Foundation import NSObject`.
8. Alternatively, download the replacement `libcxsetupbase.py` from the provided repository and replace the existing file.
9. After replacing the file, relaunch CrossOver.

Following these steps will allow you to enjoy an unlimited free trial of CrossOver.
