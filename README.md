![made-with-c++](https://img.shields.io/badge/Made_with-C%2B%2B-blue)

<!-- LOGO -->
<br />
<h1>
<p align="center">
  <img src="https://github.com/krmiller678/Project_3_Minesweeper/blob/main/Project_3_Minesweeper/images/face_win.png" alt="Logo" width="110" height="110">
  <br>Minesweeper Clone
</h1>
  <p align="center">
    C++ Minesweeper clone with Dev tools - built on SFML
    <br />
    </p>
</p>
<p align="center">
  • <a href="#about-the-project">About The Project</a> •
  <a href="#quick-start">Quick Start</a> •
  <a href="#manually-build">Build</a> •
  <a href="#usage">How to Use</a> •
  <a href="#acknowledgements">Acknowledgements</a> •
</p>  

<p align="center">
 
<img src="https://github.com/krmiller678/Project_3_Minesweeper/blob/main/Minesweeper.jpg">
</p>                                                                                                                             
                                                                                                                                                      
## About The Project
Minesweeper Clone is one of my first projects built using C++ with the Simple Fast Multimedia Library. In addition to regular game functionality, test boards are included and developer options allow for tiles to be revealed prior to game being completed.

## Quick Start
All library files are statically linked and included in the executable. Reference images are included in directories.  
[click me to download](https://github.com/krmiller678/Project_3_Minesweeper/releases/download/v1.0.0/Release.zip)

After downloading the release version, unzip the file and navigate to the `Project_3_Minesweeper.exe`. This executable will allow you to run the program.

## Manually Build

Requirements:
- Visual Studio 2015 or later
- SFML 2.5 or later

Clone from GitHub:
```
git clone https://github.com/krmiller678/Project_3_Minesweeper.git <my-directory>
```

Install Dependencies:
Windows:
```bash
vcpkg install sfml
```
Mac:
```bash
brew install sfml
```
You can also visit the official [SFML Website](https://www.sfml-dev.org/download/sfml/2.5.0/) to download any version manually.

Configure Visual Studio:  
After opening the Visual Studio `Project_3_Minesweeper.sln` file
1. Navigate to _Project_-> _Properties_-> _C/C++_-> _General_ and add in your SFML include directory under _Additional_Include_Directories_. Mine looks like this "Z:\SFML-2.5.1\include"
2. In _C/C++_-> _Preprocessor_ add in "SFML_STATIC" under _Preprocessor_Definitions_
3. Navigate to _Properties_ -> _Linker_-> _General_ and under _Additional_Library_Directives_ add in your SFML lib directory. Mine looks like this "Z:\SFML-2.5.1\lib"
4. In _Linker_ -> _Input_ under _Additional_Dependencies_ add the following:  
sfml-graphics-s.lib  
sfml-window-s.lib  
sfml-system-s.lib  
winmm.lib  
opengl32.lib  
freetype.lib
5. Build the project! 

## Usage
### Input/Output
- **Left-click** to engage with tiles and on screen elements.
- **Right-click** to mark or unmark flags.
### On Screen Buttons
- **Smiley Button** to reset the board <img src="https://github.com/krmiller678/Project_3_Minesweeper/blob/main/Project_3_Minesweeper/images/face_happy.png" alt="Logo" width="25" height="25">   

- **Peek Button** to view mines <img src="https://github.com/krmiller678/Project_3_Minesweeper/blob/main/Project_3_Minesweeper/images/debug.png" alt="Logo" width="25" height="25">   

- **Test Button** to load test cases <img src="https://github.com/krmiller678/Project_3_Minesweeper/blob/main/Project_3_Minesweeper/images/test_1.png" alt="Logo" width="25" height="25">   

### Screen Elements
- **Number Tiles** represent the number of adjacent mines.
- **Flags** mark where the user believes mines to be.
- **Counter** represents how many unmarked mines are left.


## Acknowledgements
- Credit to the [SFML Community](https://github.com/ikonikon/fast-copy) for the great wealth of knowledge.
- Credit to Professor Fox in the UF CISE department for being a great instructor.
