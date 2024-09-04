# Ys Vi: The Ark of Napishtim Decompilation
- Release: Steam NA 1.2.0.1 (Not DX9)
- Publisher: XSEED Games (2015, Windows 10)
- Original: Nihon Falcom Corp. (2003, Windows 7/8/Vista/Xp)

## The Project
Decompile Ys Vi's modern english release using Ghidra for the purpose of quality of life changes and understanding the game. As far as I am aware, I am one of the first to research modifications for this game, so there is a lot to discover. I am learning as I go, and I am making pretty steady progress in my free time.

## The Goals
- Obtain a solid understanding of the game's fundamental systems
- Replace the default HD english font (MS Gothic) with something more fitting
- Enable modifications to character portraits and music tracks
- Enable modifications to game balance

## Hopes and Dreams
- Implement the japanese dub from the PS2 release (The English dub uses Konami's translation and thus would not fit)
- Complete decompilation
## Resources and Credits
- Ys VI full sprite rip by <b>Magma MK-II</b>: https://www.spriters-resource.com/pc_computer/ysvithearkofnapishtim/
- Reverse Engineering Walkthroughs: www.youtube.com/@jeFF0Falltrades
- Video Game Hacking and Reverse Engineering Content: https://www.youtube.com/@hilltopworks
- All-in-one Reverse Engineering Software Directory: https://github.com/dsasmblr/game-hacking?tab=readme-ov-file
- Ys Vi Cheat Tables: https://fearlessrevolution.com/viewtopic.php?t=3058#google_vignette
- Ys Vi Cheat Protection: https://gamefaqs.gamespot.com/boards/918567-ys-vi-the-ark-of-napishtim/47534937
- Exploring Tokimeki Memorial: https://tetracorp.github.io/tokimeki-memorial/









## Components of the project

### Ys6_win.exe
The main executable of the game. Consists of the main game code, lots of external libraries, and DLLs related to Microsoft applications, GOG, and Steam. 
### config.exe
The supporting executable for the game that defines a lot of the game's system properties such as control bindings, display settings, effect settings, etc.
It may seem small but it is quite hefty with comparable numbers of functions and data to the main executable.
Includes an uncompressed png image of Isha in the file.
