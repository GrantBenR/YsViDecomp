# Audio
Ys Vi uses compressed **.wav** audio files for its in-game sound effects and uncompressed **.ogg** files via WuVorbis for its music and demo audio-tracks. 

# Graphics
I am working on the **DirectX 8** release of Ys Vi (Don't ask me why)

# Input
Ys Vi **DirectInput8** to manage user input

# Compression and Decompression
Ys Vi uses various libraries for this purpose:

- **Inflate library (1.1.4)** for its general file decompression (.ymo, .sct, etc.)

- **Libpng library (1.1.3)** for image decompression (textures, portraits, etc.)

- **XviD library** for handling game demo video files.

# Executable Info
Ys Vi appears to be have been compiled with Visual Studio, but I have yet to fully confirm this. The executable contains many library functions from Visual Studio 2005 and 2008 and appears to have the Microsoft Rich Text header.

# Game File Extensions
Game Asset Files:
- .SOB - Save pillar object
- .SBX - Sky box object
- .YMO - 3D game object
- .YCO - ???
- .XSO - Used to store project details in Expresso by Ultrapico for Windows apps
- .ASO - ???
- .AIA - Undef Sprite Object File
- .SCT - ???
- .SCM - ???
- .SFO - Region Fog File
- .SEF - ???
- .SEN - Region Entry File
- .SBE - ???
- .SL - Scene List File
- .SL2 - Effect Scene List File

Game Release Files:
- .FOT - Scalable Font Resource
- .NA - Contains SFX Audio Files (.wav)
- .NI - Release data file
- .NU - Release data file
- .DT - Multi-purpose data file (Font file, etc.)

Game Save Files:
- .NACCI - Save File
- .TA - Save Record File
- .TA2 - Save Record File

# Compiler
- Game Executable was likely originally compiled with some version of MinGW GCC 9.x, due to linker header and executable structure
