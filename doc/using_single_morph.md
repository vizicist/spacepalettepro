<h1>Using the Palette software with a single Sensel Morph or Erae Touch</h1>

If you have a Windows 10 machine and either a Sensel Morph or an Erae Touch,
you can use the Palette software for visuals with Resolume
without needing to install and configure any of the audio software
(a much more complicated process).  You can even do this with the demo version of Resolume Avenue 7 or Arena 7.
Here are the steps.

<ul>
<li>Install the Palette software
    <ul>
    <li>Use the latest version in
    <a href="https://github.com/vizicist/palette/tree/main/release">https://github.com/vizicist/palette/tree/main/release</a>
    </ul>
<li>Install Resolume Avenue or Arena (version 7).
    <ul>
    <li>The demo version will work okay, it just shows a watermark in the output.
    <li>In Avenue->Preferences->Video, add C:\Program Files\Palette\ffgl
    <li>In Avenue->Preferences->OSC, enable OSC Input on port 7000
    <li>Quit and restart Resolume
    <li>Verify that Palette plugin is seen in Sources under Generators
    <li>In Composition->Open, open %LOCALAPPDATA%\Palette\config\PaletteABCD.avc, then Quit
    </ul>
<li>If you have a Sensel Morph...
    <ul>
    <li>Plug it in.
    <li>Install the Sensel App, if you haven't already.
    <li>Make sure that the Morph is seen by the Sensel App, and its firmware is up-to-date.
    </ul>
<li>If you have an Erae Touch...
    <ul>
    <li>Plug it in.
    <li>Start the EraeLab application
    <li>Open %LOCALAPPDATA%\Palette\config\EraeTouchLayout.emk
    <li>Save this layout in whatever layout slot you like.
    <li>Close the EraeLab application (it can't be running at the same time as the Palette software)
    </ul>
</ul>
<p>
You've completed the installation steps.  Every time you want to use it:
<p>
<ul>
<li>In the Windows menu, invoke Palette->Start Palette (small GUI).
    <ul>
    <li>Note: the Palette Control window might be hidden behind Resolume.
    <li>If a Palette Control window doesn't appear and isn't hidden behind other windows, you can find logfiles in %LOCALAPPDATA%\Palette\logs that may help uncover the problem.
    </ul>
<li>In the Palette Control window, select one of the presets.
<li>Finger paint on the Sensel Morph or Erae Touch.  You should see visuals appear in Resolume.
<li>The four corners of the Morph (or Touch) can be used to switch
between four virtual pads, simulating the four Morphs in the Space Palette Pro.  For example, touching the lower-left corner will cause it to act
like the lower-left Morph in the real Space Palette Pro.
You can use the corners to switch at anytime.
<li>To stop both Resolume and the Palette engine (which is running in the background), use Palette->Stop Palette in the Windows menu.
</ul>