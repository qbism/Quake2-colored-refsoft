# Quake2-colored-refsoft
ref_soft.dll for Quake2 with colored lighting in context of Knightmare's Unofficial Q2 Patch.

This is a replacement ref_soft.dll adding colored lighting and widescreen waterwarp support to the Quake 2 software renderer. Alphatest and transparency are improved as a bonus. darklights work. Not to mention the ddraw palette problem fixed- this one only uses DIB even for fullscreen! Knightmare’s ‘unofficial Q2 patch’ 3.24 is supported, although haven’t tried it on any others.

Oh, yeah, and there’s a cvar called ‘sw_transmooth’ that dithers transparent surfaces.

Download dll: _extfiles/ref_soft_color.zip 

Source code: _extfiles/ref_soft_color_src.zip 

Notes about the code- It can be copied into the 3.24 source folder. (Make a backup for this purpose.) But I don’t have VC 6, so I built it with VS 2013 (project included in the ref_soft folder).
This started with the colored light code leilei added to stock Q2. Shaded light was completed among other things with head-scratching and borrowed pieces of engoo. Waterwarp improvement and dithering are from AROS Quake2.

Q: Can The Reckoning run?
A: Try creating a shortcut instead of the .bat file. I do C:\quake2\quake2_324.exe +set game xatrix (I renamed knightmare’s 3.24 to this). Also let the xatrix logo intro vid play through, but can skip the cutscene vid.

Q: How can bilinear (smooth) filtering be disabled for water?
A: sw_transmooth 0

