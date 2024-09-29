# Audio
Ys Vi uses compressed **.wav** audio files for its in-game sound effects and uncompressed **.ogg** files via WuVorbis for its music and demo audio-tracks. 

# Graphics
Ys Vi uses **Direct3D and DirectX 8** for its rendering

# Input
Ys Vi uses **DirectInput8** to manage user input

# Compression and Decompression
Ys Vi uses various libraries for this purpose:

- **Inflate library (1.1.4)** for its general file decompression (.ymo, .sct, etc.)

- **Libpng library (1.1.3)** for image decompression (textures, portraits, etc.)

- **XviD library** for handling game demo video files.

# Game File Extensions

Game Asset Files:
- .SOB - Save pillar object
- .SBX - Sky box object
- .YMO - 3D game object
- .SCT - ???
- .SCM - ???
- .SFO - Game Map Component
- .SEF - ???
- .SEN - ???
- .SBE - ???
- .SL - Scene List File
- .SL2 - Effect Scene List File

Game Release Files:
- .FOT - Scalable Font Resource
- .NA - Release data file
- .NI - Release data file
- .NU - Release data file
- .DT - Multi-purpose data file (Font file, etc.)

Game Save Files:
- .NACCI - Save File
- .TA - Save Record File
- .TA2 - Save Record File

