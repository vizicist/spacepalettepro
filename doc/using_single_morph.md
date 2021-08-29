<h1>Using the Palette software with a single Morph</h1>

If you have a single Sensel Morph and a Windows 10 machine,
you can use the Palette software for visuals with Resolume
without needing to install and configure any of the audio software
(a much more complicated process).  You can even do this with the demo version of Resolume Avenue 7 or Arena 7.
Here are the steps to do that.

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
<li>Plug in the Morph
    <ul>
    <li>Install the Sensel App, if you haven't already.
    <li>Make sure that the Morph is seen by the Sensel App, and its firmware is up-to-date.
    </ul>
</ul>
<p>
You've completed the one-time steps.  To use it:
<p>
<ul>
<li>In the Windows menu, invoke Palette->Start Palette (small GUI).
    <ul>
    <li>Note: the Palette Config window might be hidden behind Resolume when it first starts.
    <li>If a Palette Config window doesn't appear and isn't hidden behind other windows, you can find logfiles in %LOCALAPPDATA%\Palette\logs that may help uncover the problem.
    </ul>
<li>In the Palette Config window, select one of the presets.
<li>Finger paint on the Morph.  You should see visuals appear in Resolume.
<li>The four corners of the single Morph can be used to switch
between four virtual pads, simulating the four Morphs in the Space Palette Pro.  For example, touching the lower-left corner of
the Morph will cause it to act
like the lower-left Morph in the real Space Palette Pro.
You can use the corners to switch at anytime.
</ul>