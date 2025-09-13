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

<li>Download and install Chrome, then sign in as spacepalette@gmail.com.  Let it create a passkey.  Do not turn on sync or anything else.

<li>In Chrome, go to remotedesktop.google.com and seleromet "Access My Computer".  Scroll down and "Set up remote access".  Install the remotedesktop extension in Chrome, and use spacepalette{serialnum} for the computer name.

<li>Set Chrome as the default browser.  Set chrome startup to "where you left off"

<li>Download and install Windows updates.

<li>In Windows->Settings->Accounts->Sign-in options, under "Additional settings" turn off "...only allow Windows Hello..."

<li>Use Win-R to run netplwiz.exe, and set it up to automatically log in with spacepalette{serialnum}@outlook.com

<li>Reboot to make sure autologon works.

<li>Show filename extensions in Explorer
<li>Install sharpkeys to remap capslock key.
<li>Install WSL and Ubuntu
<li>Install Github Desktop
<li>Install cli.github.com
<li>cd %USERPROFILE%\Github, gh repo clone vizicist/palette
<li>cd %USERPROFILE%\Github, gh repo clone vizicist/spacepalettepro
<li>Install release/palette_win_setup_{latest}
<li>Install release/palette_data_default_{latest}
<li>Install SenselApp0.19.32
<li>Install vim (create .bat files)
<li>Install 7zip
<li>Install Go
<li>Install Visual Studio Code
<li>Install Visual Studio Community edition
<li>Install Resolume 7, license it, Enable OSC input, set Video Plugin dir to c:\Program Files\Palette\ffgl
<li>In Resolume, open c:\Program Files\Common Files\Palette\data_default\config\PaletteDefault.avc
<li>Install Drumnet
<li>Install Plogue BIdule, enable OSC server, set VST path to c:\Program Files\Common Files\VST3
<li>Install LoopBe, disable shortcut protection, expand to 16 ports

<li>Follow the instructions for <a href="building_software.md">building the software</a>.
</ol>
