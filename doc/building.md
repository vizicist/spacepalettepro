<h1>Building the Space Palette Pro</h1>
These are the steps to building a complete system.
<p>
<ul>
<li>Buy all the parts
<li>Cut the wood pieces
<li>Put together the controller
<li>Put together the monitor
<li>Put together the base
<li>Attached the monitor and controller to the base
<li>Install commercial software
<li>Install open-source software
</ul>
Each of those steps is described below.
<p>

<h1>Buy all the parts</h1>
The <a href="parts.ods"><code>parts.ods</code></a> file is a
spreadsheet listing all of the non-wood parts needed.
<a href="parts.pdf"><code>parts.pdf</code></a> is a large printable version, and
if you download this PDF and display it in your browser, the links will
be enabled and point to the places (mostly Amazon) where you can buy each piece.

<h1>Cut the wood pieces</h1>
A list of the wood pieces with pictures of each can be found in <a href="../dxf/list.md"><code>dxf/list.md</code></a>.
The <a href="../dxf/list.txt"><code>dxf/list.txt</code></a> file is a more concise list
that shows for each piece the quantity, thickness, and DXF filename.
Most of these pieces should be baltic birch, but some of them can be another material.
For example, some CNC services may not support cutting 1/8" baltic birch, and
so you can use another material for those.
For the top layer of the controller (SPP_Layer1_face.dxf) and the top layer
of the monitor (SPP_MonLayer1_face.dxf), you might consider using
<a href="https://www.buyappleply.com/">ApplePly</a> for a nicer wood appearance.

<h1>Put together the controller</h1>
Here are some <a href="https://photos.app.goo.gl/FhGk2NVdA6P4zqocA">pictures showing the controller build process.</a>

<h1>Put together the monitor</h1>
Here are some <a href="https://photos.app.goo.gl/Fwk42kaN5rRdKyEm8">pictures showing the monitor build process.</a>

<h1>Put together the base</h1>
Here are some <a href="https://photos.app.goo.gl/kpxXuAgzLdUquVTU9">pictures showing the base build process.</a>

<h1>Setup Windows and install software</h1>

1) Change computer name to palette{serialnum}
2) Reboot, put in USB wifi, connect to network
3) Use Microsoft account to log in, install Windows udpates
4) Install Chrome, enable google remote desktop (requires Google account)
5) Install LoopBe30 from https://www.nerds.de/en/order.html 
    - Use LoopBe30 tray to expand "ports after reboot" to 16
    - Turn off "Enable Shortcut Detection"
    - Reboot
6) Install Palette version 5.1
7) Install Omnisphere in c:\users\public\documents\vstplugins64
8) Install Battery 4 in c:\users\public\documents\vstplugins64
9) Install Battery 4 Factory Library
10) Install Plogue Bidule:
    - In Edit->Preferences->VST add folder c:\users\public\documents\vstplugins64
    - In Tools->Osc Server enable OSC 
    - Read %LOCALAPPDATA%\Palette\config\palette.bidule
    - Make sure Battery 4 instances can send audio, fix audio device if necessary
    - Authorize Omnisphere
    - Restart Bidule, verify that Omnisphere is authorized
11) Install Resolume 7 (Avenue)  
    - In Avenue->Preferences->Video, add C:\Program Files\Palette\ffgl
    - In Avenue->Preferences->OSC enable OSC Input on port 7000
12) Install SenselApp