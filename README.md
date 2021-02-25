# OptimizationWindowsV1

Powershell script for optimizations, tweaks & bloatware. Short script ps1 for remove the unnecessary part on Windows 10

# Warning !

I do not take responsibility for what may happen to your system. This is at your own risk.
Think to check the Ninite part (programm that make you install automatically few programms) and adapt it to what you need/use/want.

# How To Run the OptimizationWindowsV1.ps1 file :

  1. Download the .zip file on the main page of the github and extract the .zip file to your desired location.
  2. Once extracted, open PowerShell ISE as an Administrator (Really important).
  3. Read all the functions proposed by the script and adapt them according to your needs.
  4. Press F5 when you're ready to launch the script for execute it.

# Switch Parameters :

For switch parameters you just need to add a # in front of a function. You actually don't need to touch what is
under line 223.

  The first one is -SysPrep, which runs the command within a function: get-appxpackage | remove-appxpackage. This is useful since some administrators need that command to run      first in order for machines to be able to properly provision the apps for removal.
    The second switch parameter is -Debloat, which does as it suggests. It runs the following functions: Start-Debloat, Remove-Keys, and Protect-Privacy.
    Remove-Keys removes registry keys leftover that are associated with the bloatware apps listed above, but not removed during the Start-Debloat function.
    Third, Protect-Privacy adds and/or changes registry keys to stop some telemetry functions, stops Cortana from being used as your Search Index, disables "unneccessary"        scheduled tasks, and more.

These scheduled tasks that are disabled have absolutely no impact on the function of the OS.

  To reverse the functions you have touched simply add/remove the # in front of a function you have modified.

# Blotaware that is removed :

3DBuilder, ActiproSoftware, Alarms, Appconnector, Asphalt8, Autodesk SketchBook, Bing Finance, Bing Food And Drink, Bing Health And Fitness, Bing News, Bing Sports, Bing Travel, Bing Weather, BioEnrollment, Camera, CandyCrush, CandyCrushSoda, Caesars Slots Free Casino, ContactSupport, CyberLink MediaSuite Essentials, DrawboardPDF, Duolingo, EclipseManager, Facebook, FarmVille 2 Country Escape, Flipboard, Fresh Paint, Get started, iHeartRadio, King apps, Maps, March of Empires, Messaging, Microsoft Office Hub, Microsoft Solitaire Collection, Microsoft Sticky Notes, Minecraft, Netflix, Network Speed Test, NYT Crossword, Office Sway, OneNote, OneConnect, Pandora, People, Phone, Phototastic Collage, PicsArt-PhotoStudio, PowerBI, Royal Revolt 2, Shazam, Skype for Desktop, SoundRecorder, TuneInRadio, Twitter, Windows communications apps, Windows Feedback, Windows Feedback Hub, Windows Reading List, XboxApp, Xbox Game CallableUI, Xbox Identity Provider, Zune Music, Zune Video.
