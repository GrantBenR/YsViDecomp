# Ys VI: The Ark of Napishtim Decompilation
- Release: Steam North America 1.2.0.1 (DirectX8 version)
- Publisher: XSEED Games (2015, Windows 10)
- Original: Nihon Falcom Corp. (2003, Windows 7/8/Vista/Xp)

## The Project
Decompile Ys Vi's modern english release using Ghidra for the purpose of quality of life changes and understanding the game. As far as I am aware, I am one of the first to research modifications for this game, so there is a lot to discover. I am learning as I go, and I am making pretty steady progress in my free time.

## The Goals
- Obtain a solid understanding of the game's fundamental systems
- Replace the default HD english font (MS Gothic) with something more fitting
- Enable modifications to character portraits and sfx
- Enable modifications to game balance

## Hopes and Dreams
- Implement the japanese dub from the PS2 release (The English dub uses Konami's translation and thus would not fit)
- Complete decompilation
## Resources and Credits
### - Ys VI full sprite rip by <b>Magma MK-II</b>: https://www.spriters-resource.com/pc_computer/ysvithearkofnapishtim/
  Magma's work sprite ripping this game was incredibly useful at many points in the reverse engineering process and I am very thankful for it.
### - Reverse Engineering Walkthroughs: www.youtube.com/@jeFF0Falltrades
  His videos were pivotal to my early learning in Ghidra and I am highly appreciative for his in-depth tutorials.
### - Video Game Hacking and Reverse Engineering Content: https://www.youtube.com/@hilltopworks
  Hilltop has worked on a ton of excellent game modding projects over the years and has made many highly informative videos on the topic. His work has been inspiring to me and I am profoundly thankful for the work he's doing.
### - Psound201
  Software for converting .VAG files to .WAV.
### -  MediaExtract by @Panzi - https://github.com/panzi/mediaextract
  Used to rip sfx from .NA release file
### - Pycave by Alexandre Cheron - https://github.com/axcheron/pycave
Used to find code caves in the executable
### - Binocle by Sharkdp - https://github.com/sharkdp/binocle/releases/tag/v0.3.2
Used to analyze visually release files
### - All-in-one Reverse Engineering Software Directory: https://github.com/dsasmblr/game-hacking?tab=readme-ov-file
### - Ys Vi Cheat Tables: https://fearlessrevolution.com/viewtopic.php?t=3058#google_vignette
### - Ys Vi Cheat Protection: https://gamefaqs.gamespot.com/boards/918567-ys-vi-the-ark-of-napishtim/47534937
### - Exploring Tokimeki Memorial: https://tetracorp.github.io/tokimeki-memorial/



## Progress Report - 9-22-24
- Function identification: more than <b>50%</b> of the functions have been classified. Many main game functions have been fully identified!
- Sfx identification: less than 40% identified
- Vfx identification: less than 30% identified
- Bgm identification: <b>full identification!</b>
- Gamemap Models identification: <b>full identification!</b>
- I am still working my way around the edges of the puzzle so to speak. Much of the main gameplay functions have been found, but most of the complex structures like the game's rendering and decompression solutions need to be researched further.
## Progress Report - 9-26-24
- Function identification: now **more than 75%!**
- Almost all enemy actor's functions have been identified
- As before, I still have a ton to learn. The majority of unclassified functions still remaining I believe are related to Direct3D, decompression, or just junk compiler code. Overall, I am very blessed to have the free time to continue with this project, and I pray that God can continue to provide me the same motivation and opportunities.
## Progress Report - 10-3-24
- Function Identification: Only **900** functions left unclassified!
- All bespoke game classes have been identified. All the particulars of what GoXx does have yet to be understood.
- Decompression libraries have been identified, and I am working on using this info to dump the game's non-png assets
## Progress Report - 10-13-24
- No significant change on function identification. The remaining are rather hard to define and mostly relate to the particulars of decompression and visual effects.
- I was able to rip the game's sfx and was also able to rip the Japanese voice acting files from the Konami PS2 release of the game as .wav files (all 4200 of em yikes!).
- More research needed into how the game dialog is triggered in order to potentially implement voice acting
## Progress Report - 10-15-24
- There is a 400 byte "code cave" starting at 52C924 that I believe would be ideal for inserting a potential new dialog function for voice acting.
- I have managed to identify the majority of sfx files for the game, though some unlabeled enemy attack sfx I still don't get.
## Progress Report - 11-10-24
- Just under 700 functions remaining. So, so, so . . . so, so so many direct3d and decompression functions that I cannot make any sense of at the moment.
- I need to research more about patching executables in ghidra in regards to patching data rather than instructions.
- Still learning how I want to pace my work on this project
## Progress Report - 11-11-24
- So I locked in, and now only **200** functions remain to be classified! Turns out, there were at least 500 decompression related functions in this game, and though I do not fully understand the process yet I was able to classify them by decompression type for the most part.
## Progress Report - 11-14-24
- WE'VE REACHED DOUBLE DIGITS BABY WOOOOOO!!!! Just 98 functions remaining. They appear to primarily be complex sub functions for vfx and particle fx, and I'm working through identifying them pretty steadily
- That being said, here are the next steps:
- Figure out how game scenes and dialog are triggered in order to implement voice acting, likely involving extracting the scenelist.sl file.
- Patch a new function to load dialog audio files that will as of now use uncompressed audio files similar to how the BGM is played.
- Further out, given enough free time, I will more thoroughly label the data and begin proper decompilation of the game.
## Progress Report - 11-15-24
- **COMPLETE FUNCTION CLASSIFICATION**. Praise God for giving me the free time and motivation to make it this far.
- Many of the classifications are innaccurate and much more work is due in order to clarify the purpose of many gameplay functions
## Progress Report - 11-15-24
- I have made some progress on the voice acting func, however it is far from finished and I need more practice writing in assembly.
- I converted the files into OGG so that I could reuse the bgm audio functions, rather than using the wav player used for other soundeffects, and also removed the header of "V_" to "V50_" from all relevent files.
- Due to Xseed's new localization, I may need to either replace some file names with their relocalized names or just replace them entirely with the character # used in dialog
  
