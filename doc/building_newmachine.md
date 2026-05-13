<h1>Setting up Space Palette Pro on a new computer</h1>
These steps are designed for taking a new Windows 11 computer and configuring everything from scratch.
This is specific to the 2024 Asus NUC 970, but should be almost identical for most Windows computers.
<p>

<ol>

<li>When booting for the first time, keep pressing F2 until the BIOS setup comes up.  Go into the Power settings, and then select the Secondary Power Settings.  Change the "After Power Failure" setting to Power On.  Save and exit/reboot.

<li>Do the initial Windows setup and connect to a network.

<li>Change computer name to spacepalette{serialnum}.  It will reboot and install updates.

<li>When asked to log in, click on create a new account, and then "Get a new email address".
Use spacepalette{serialnum}@outlook.com / ThereIsNoPalette{serialnum}InSpace!

<li>Set up as a new PC, don't install anything else.

<li>Uninstall OneDrive.

<li>Forward email from spacepalette{serialnum}@outlook.com to me@timthompson.com

<li>Download and install Chrome, then sign in as spacepalette@gmail.com.  Let it create a passkey.  Do not turn on sync or anything else.

<li>In Chrome, go to remotedesktop.google.com and seleromet "Access My Computer".  Scroll down and "Set up remote access".  Install the remotedesktop extension in Chrome, and use spacepalette{serialnum} for the computer name.

<li>Set Chrome as the default browser.  Set chrome startup to "where you left off"

<li>Download and install Windows updates.

<li>In Windows->Settings->Accounts->Sign-in options, under "Additional settings" turn off "...only allow Windows Hello...", and set "If you've been away, when should Windows..." to "Never"

<li>Use Win-R to run netplwiz.exe, and set it up to automatically log in with spacepalette{serialnum}@outlook.com

<li>Reboot to make sure autologon works.
<li>In Windows Settings, set System->Power->Power Mode to Best Performance
<li>In Windows Settings, set System->Power->Screen timeouts to Never
<li>Increase mouse pointer size
<li>Right-click on desktop and don't show desktop icons.
<li>Set display background to solid color.

<li>Show filename extensions in Explorer
<li>Copy T:\tjt\media\spacepalettepro\palette_installers to Downloads
<li>Execute bginfo64.exe and load palette.bgi
<li>Install sharpkeys to remap capslock key.
<li>Install WSL and Ubuntu, set root to same password as Windows login
<li>Install Github Desktop
<li>Install Git for Windows
<li>Install github (gh) CLI, i.e. gh_*.msi
<li>mkdir %USERPROFILE%\Github
<li>execute "gh auth login"
<li>cd %USERPROFILE%\Github, gh repo clone vizicist/palette
<li>cd %USERPROFILE%\Github, gh repo clone vizicist/spacepalettepro
<li>Install release/palette_{release}_win_setup.exe
<li>Install release/palette_{release}_data_default.exe
<li>In your Environment Variables:
<br>- Add %USERPROFILE%\Github\palette\scripts to your PATH
<br>- Add C:\Program Files\Git\bin to your PATH
<br>- Add C:\Program Files\Git\usr\bin to your PATH
<br>- Add %USERPROFILE%\mingw64\bin to your PATH (adjust path if installed elsewhere)
<br>- Add the following new environment variables:
<br>      PALETTE=%LOCALAPPDATA%\Programs\Palette   # palette_win_setup should have already added
<br>      PALETTE_DATAROOT=%LOCALAPPDATA%\Palette   # palette_win_setup should have already added
<br>      PALETTE_SOURCE=%USERPROFILE%\Github\palette
<li>Install mingw64 to get the gcc compiler.
The last time I installed it from https://github.com/niXman/mingw-builds-binaries, and it may be necessary to download
the "online installer" and execute it from the Explorer, selecting "more info" to allow installation of an unsigned pack
age.  The options I used are: version 13.2.0, architecture 64 bit, thread model posix, rev1, ucrt.
The version of gcc I'm using gives this output from 'gcc --version' -
gcc (x86_64-win32-seh-rev1, Built by MinGW-Builds project) 14.2.0

<li>Install Python 3.{latest} from python.org (NOT windows store), and add it to PATH, and disable PATH limit
<li>Install InnoSetup
<li>Install SenselApp0.19.32
<li>Install gvim (create .bat files)
<li>Install 7zip
<li>Install Go
<li>In palette repo, run go mod tidy
<li>Install Visual Studio Code, install vim and go extensions, update to latest
<li>Some of the installers (e.g. Visual Studio) seem to require a real HDMI to be plugged in
<li>Install Visual Studio Community edition, selecting "Desktop development with C++"
<li>Install Resolume 7, license it, Enable OSC input, set Video Plugin dir to %LOCALAPPDATA%\Programs\Palette\ffgl
<li>In Resolume, open %LOCALAPPDATA%\Palette\data_default\config\PaletteDefault.avc
<li>Create c:\Program Files\Common Files\VST2 and VST3
<li>Install Drumnet
<li>Install Omnisphere and license it with spacepalette{serialnum}@outlook.com
<li>Install Plogue Bidule (version 9784 or later), enable OSC server
<li>Install LoopBe, disable shortcut protection, expand to 16 ports
<li>Run scripts/multitouch_disable.bat
<li>Run scripts/setup_onboot.bat (as administrator)
<li>With touchscreen connected, Control Panel->small icons->Tablet PC Settings, Setup, Touch Settings.
<li>In Display Settings, put touchscreen to left of main screen, and Portrait Flipped.
<li>cd palette\build\windows ; build & install
<li>palette setboot global.guisize palette
</ol>
