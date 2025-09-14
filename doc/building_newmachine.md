<h1>Building the Software of the Space Palette Pro</h1>
These steps are designed for taking a new Windows 11 computer and configuring everything from scratch.
This is specific to the 2024 Asus NUC 970, but should be almost identical for most Windows computers.
<p>

<ol>

<li>When booting for the first time, keep pressing F2 until the BIOS setup comes up.  Go into the Power settings, and then select the Secondary Power Settings.  Change the "After Power Failure" setting to Power On.  Save and exit/reboot.

<li>Do the initial Windows setup and connect to a network.

<li>Change computer name to spacepalette{serialnum}.  It will reboot and install updates.

<li>When asked to log in, click on create a new account, and then "Get a new email address".
Use spacepalette{serialnum}@outlook.com / ThereIsNoPalette{serialnum}InSpace.

<li>Set up as a new PC, don't install anything else.

<li>Uninstall OneDrive.



<li>Download and install Chrome, then sign in as spacepalette@gmail.com.  Let it create a passkey.  Do not turn on sync or anything else.

<li>In Chrome, go to remotedesktop.google.com and seleromet "Access My Computer".  Scroll down and "Set up remote access".  Install the remotedesktop extension in Chrome, and use spacepalette{serialnum} for the computer name.

<li>Set Chrome as the default browser.  Set chrome startup to "where you left off"

<li>Download and install Windows updates.

<li>In Windows->Settings->Accounts->Sign-in options, under "Additional settings" turn off "...only allow Windows Hello..."

<li>Use Win-R to run netplwiz.exe, and set it up to automatically log in with spacepalette{serialnum}@outlook.com

<li>Reboot to make sure autologon works.
<li>In Windows Settings, set System->Power->Power Mode to Best Performance
<li>In Windows Settings, set System->Power->Screen timeouts to Never

<li>Show filename extensions in Explorer
<li>Install sharpkeys to remap capslock key.
<li>Install WSL and Ubuntu
<li>Install Github Desktop
<li>Install cli.github.com
<li>cd %USERPROFILE%\Github, gh repo clone vizicist/palette
<li>cd %USERPROFILE%\Github, gh repo clone vizicist/spacepalettepro
<li>Install release/palette_win_setup_{latest}
<li>Install release/palette_data_default_{latest}
<li>In your Environment Variables:
- Add %USERPROFILE%\Github\palette\scripts to your PATH
- Add C:\Program Files\Git\bin to your PATH
- Add C:\Program Files\Git\usr\bin to your PATH
- Add %USERPROFILE%\mingw64\bin to your PATH (adjust path if installed elsewhere)
- Add the following new environment variables:
```
 PALETTE=C:\Program Files\Palette
 PALETTE_SOURCE=%USERPROFILE%\Github\palette
```
<li>Install mingw64 to get the gcc compiler.
The last time I installed it from https://github.com/niXman/mingw-builds-binaries, and it may be necessary to download
the "online installer" and execute it from the Explorer, selecting "more info" to allow installation of an unsigned pack
age.  The options I used are: version 13.0, architecture 64 bit, posix, rev1, ucrt.
The version of gcc I'm using gives this output from 'gcc --version' -
gcc (x86_64-win32-seh-rev1, Built by MinGW-Builds project) 14.2.0

<li>Install Python 3.{latest} from python.org (NOT windows store), and add it to PATH
<li>Install InnoSetup
<li>Install SenselApp0.19.32
<li>Install vim (create .bat files)
<li>Install 7zip
<li>Install Go
<li>In palette repo, run go mod tidy
<li>Install Visual Studio Code, install vim and go extensions
<li>Install Visual Studio Community edition
<li>Install Resolume 7, license it, Enable OSC input, set Video Plugin dir to c:\Program Files\Palette\ffgl
<li>In Resolume, open c:\Program Files\Common Files\Palette\data_default\config\PaletteDefault.avc
<li>Install Drumnet
<li>Install Omnisphere.
<li>Install Plogue Bidule (version 9784 or later), enable OSC server, set VST path to c:\Program Files\Common Files\VST3
<li>Install LoopBe, disable shortcut protection, expand to 16 ports
<li>Run scripts/multitouch_disable.bat
<li>Run scripts/setup_onboot.bat (as administrator)

<li>Follow the instructions for <a href="building_software.md">building the software</a>.
</ol>
