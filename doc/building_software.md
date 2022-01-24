<h1>Building the Software of the Space Palette Pro</h1>
These are the steps to install and configure all the necessary software for a full-blown (visuals and sound) Space Palette Pro.  This procedure is much more complex than it is for a visuals-only Space Palette Pro.  If you only want to do visuals, the much simpler installation procedure is at
<a href="https://github.com/vizicist/palette/blob/main/docs/using_resolume.md">https://github.com/vizicist/palette/blob/main/docs/using_resolume.md</a>
<p>

<ol>
<li>Install LoopBe30 from <a href="https://www.nerds.de/en/order.html">https://www.nerds.de/en/order.html</a><br>
    <ul>
    <li>Use LoopBe30 tray item to expand "ports after reboot" to 16
    <li>Turn off "Enable Shortcut Detection"
    <li>Reboot
    </ul>
<li>Install Palette
    <ul>
    <li>The latest version in
    <a href="https://github.com/vizicist/palette/tree/main/release">https://github.com/vizicist/palette/tree/main/release</a>
    </ul>
<li>Install Omnisphere 2 in c:\users\public\documents\vstplugins64
<li>Install Battery 4 in c:\users\public\documents\vstplugins64
<li>Install Battery 4 Factory Library
<li>Install Plogue Bidule:
    <ul>
    <li>In Edit->Preferences->VST add folder c:\users\public\documents\vstplugins64
    <li>In Tools->Osc Server, enable OSC 
    <li>Open %LOCALAPPDATA%\Palette\config\palette.bidule
    <li>Make sure Battery 4 instances can send audio, fix audio device if necessary
    <li>Authorize Omnisphere 2
    <li>Restart Bidule, verify that Omnisphere is authorized
    </ul>
<li>Install Resolume 7 (Avenue)  
    <ul>
    <li>In Avenue->Preferences->Video, add C:\Program Files\Palette\ffgl
    <li>In Avenue->Preferences->OSC, enable OSC Input on port 7000
    <li>Quit and restart Resolume
    <li>Verify that Palette plugin is seen in Sources under Generators
    <li>In Composition->Open, open %LOCALAPPDATA%\Palette\config\PaletteABCD.avc, then Quit
    <li>In Output->Fullscreen, set the Palette's main monitor to fullscreen
    </ul>
<li>Install SenselApp
    <ul>
    <li>Verify that all Morphs are seen
    <li>Make sure their serial numbers are in %LOCALAPPDATA%\Palette\config\morphs.json
    </ul>
<li>Install Git from <a href="https://gitforwindows.org">https://gitforwindows.org</a><br>
    <ul>
    <li>Accept all the defaults
    <li>adjust PATH to add c:\program files\git\usr\bin
    <li>Optional: install GitHub Desktop from <a href="https://desktop.github.com">https://desktop.github.com</a>
    </ul>
</ol>
If you are using a touchscreen monitor for the preset selector GUI, then do these steps:
<p>
<ol>
<li>Use Windows Settings->Display to adjust the monitor settings
    <ul>
    <li>Adjust touchscreen monitor for Resolution = 800x1280, Orientation = Portrait (flipped)
    <li>Put console monitor on the right, touchscreen monitor in the middle, and the external monitor (or oval monitor) on the left.
    </ul>
<li>Make sure Windows knows which monitor is the touchscreen
    <ul>
    <li>Go to the Windows Control Panel (the old one)
    <li>change the "View by" to "Small icons"
    <li>In "Tablet PC Settings", select "Setup..." and then "Touch Input",
      selecting the touchscreen monitor as the touch screen
    <li> If you don't see "Tablet PC Settings", it means the touchscreen monitor
      isn't connected.
    </ul>
</ol>
