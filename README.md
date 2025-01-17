```ps1

# Check ExecutionPolicy 
Get-ExecutionPolicy -List

# Set ExecutionPolicy to Bypass for CurrentUser
Set-ExecutionPolicy Bypass -Scope CurrentUser

# Install chocolatey
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

# Install packages from chocolatey.config
choco install chocolatey.config -y

# Install wsl
wsl --install

Restart-Computer
```

[windows autoanswers config](https://schneegans.de/windows/unattend-generator/?LanguageMode=Unattended&UILanguage=en-US&Locale=en-US&Keyboard=00000409&UseKeyboard2=true&Locale2=ru-RU&Keyboard2=00000419&GeoLocation=244&ProcessorArchitecture=amd64&BypassRequirementsCheck=true&ComputerNameMode=Random&CompactOsMode=Never&TimeZoneMode=Explicit&TimeZone=Ekaterinburg+Standard+Time&PartitionMode=Interactive&WindowsEditionMode=Generic&WindowsEdition=pro&UserAccountMode=Unattended&AccountName0=Admin&AccountPassword0=&AccountGroup0=Administrators&AccountName1=&AccountName2=&AccountName3=&AccountName4=&AutoLogonMode=Own&PasswordExpirationMode=Unlimited&LockoutMode=Default&HideFiles=HiddenSystem&ShowFileExtensions=true&ClassicContextMenu=true&LaunchToThisPC=true&TaskbarSearch=Hide&TaskbarIconsMode=Empty&DisableWidgets=true&HideTaskViewButton=true&DisableBingResults=true&StartTilesMode=Default&StartPinsMode=Empty&DisableSystemRestore=true&EnableLongPaths=true&PreventAutomaticReboot=true&DisableAppSuggestions=true&DisablePointerPrecision=true&DeleteWindowsOld=true&EffectsMode=Default&WifiMode=Skip&ExpressSettings=DisableAll&KeysMode=Skip&ColorMode=Custom&SystemColorTheme=Dark&AppsColorTheme=Dark&AccentColor=%230078d4&WallpaperMode=Solid&WallpaperColor=%23000000&Remove3DViewer=true&RemoveBingSearch=true&RemoveClipchamp=true&RemoveClock=true&RemoveCopilot=true&RemoveCortana=true&RemoveDevHome=true&RemoveFamily=true&RemoveFeedbackHub=true&RemoveGetHelp=true&RemoveHandwriting=true&RemoveInternetExplorer=true&RemoveMailCalendar=true&RemoveMaps=true&RemoveMathInputPanel=true&RemoveMediaFeatures=true&RemoveMixedReality=true&RemoveZuneVideo=true&RemoveNews=true&RemoveOffice365=true&RemoveOneDrive=true&RemoveOneNote=true&RemoveOneSync=true&RemoveOpenSSHClient=true&RemoveOutlook=true&RemovePaint=true&RemovePaint3D=true&RemovePeople=true&RemovePowerAutomate=true&RemovePowerShellISE=true&RemoveQuickAssist=true&RemoveRecall=true&RemoveRdpClient=true&RemoveSkype=true&RemoveSnippingTool=true&RemoveSolitaire=true&RemoveSpeech=true&RemoveStepsRecorder=true&RemoveStickyNotes=true&RemoveTeams=true&RemoveGetStarted=true&RemoveToDo=true&RemoveVoiceRecorder=true&RemoveWallet=true&RemoveWeather=true&RemoveFaxAndScan=true&RemoveWindowsHello=true&RemoveWindowsMediaPlayer=true&RemoveZuneMusic=true&RemoveWordPad=true&RemoveXboxApps=true&RemoveYourPhone=true&WdacMode=Skip)

[dvorak-qwerty source](https://github.com/bradfeehan/Dvorak-QWERTY-Ctrl)
