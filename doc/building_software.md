<h1>Building the Software of the Space Palette Pro</h1>
These steps are designed for taking a new Windows 10 computer and configuring everything from scratch.
<p>

<ol>
<li>Change computer name to palette{serialnum}
<li>Reboot, put in USB wifi, connect to network
<li>Use Microsoft account to log in, install Windows udpates
<li>Install Chrome
    - Optionally: enable google remote desktop.  This requires a Google account, and is very useful for remote installation and monitoring.
<li>Install LoopBe30 from https://www.nerds.de/en/order.html 
    - Use LoopBe30 tray item to expand "ports after reboot" to 16
    - Turn off "Enable Shortcut Detection"
    - Reboot
<li>Install Palette
    - The latest version in https://github.com/vizicist/palette/tree/main/release
<li>Install Omnisphere 2 in c:\users\public\documents\vstplugins64
<li>Install Battery 4 in c:\users\public\documents\vstplugins64
<li>Install Battery 4 Factory Library
<li>Install Plogue Bidule:
    - In Edit->Preferences->VST add folder c:\users\public\documents\vstplugins64
    - In Tools->Osc Server enable OSC 
    - Open %LOCALAPPDATA%\Palette\config\palette.bidule
    - Make sure Battery 4 instances can send audio, fix audio device if necessary
    - Authorize Omnisphere 2
    - Restart Bidule, verify that Omnisphere is authorized
<li>Install Resolume 7 (Avenue)  
    - In Avenue->Preferences->Video, add C:\Program Files\Palette\ffgl
    - In Avenue->Preferences->OSC enable OSC Input on port 7000
    - Quit and restart Resolume
    - Verify that Palette ffgl plugin is seen in Sources under Generators
    - In Composition->Open, open %LOCALAPPDATA%\Palette\config\PaletteABCD.avc, then Quit
    - In Output->Fullscreen, set Display 3 (the Palette's main monitor) to fullscreen
<li>Install SenselApp
    - Verify that all 4 Morphs are seen
    - Make sure their serial numbers are in %LOCALAPPDATA%\Palette\config\morphs.json
<li>Install Git from https://gitforwindows.org
    - Accept all the defaults
    - adjust PATH to add c:\program files\git\usr\bin
    - Optional: install GitHub Desktop from https://desktop.github.com
<li>Use Windows Settings->Display to adjust windows
    - Adjust touchscreen monitor - Resolution = 800x1280, Orientation = Portrait (flipped)
    - Put console monitor on the right, touchscreen monitor in the middle,
      and the main (oval) monitor on the left.
<li>In the Windows Control Panel (the old one)
    - change the "View by" to "Small icons"
    - In "Tablet PC Settings", select "Setup..." and then "Touch Input",
      selecting the touchscreen monitor as the touch screen
    - If you don't see "Tablet PC Settings", it means the touchscreen monitor
      isn't connected,
<li>Run everything
    - Execute palettestartall
</ol>