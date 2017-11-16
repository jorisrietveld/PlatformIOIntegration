# Embedded and IOT Development plugin
>I always wanted to create an plugin for jetbrains to learn about there plugin system and dive deeper 
in Java development. For embedded development I often use [Clion](https://www.jetbrains.com/clion/) for writing the code in combination 
with [PlatformIO Core](http://docs.platformio.org/en/latest/core.html) for uploading the code to my Arduino, Atmega32 and other embedded development 
boards/MicroControllers. I really enjoy PlatformIO but I don't feel quite comfortable using there [complete 
IDE](http://docs.platformio.org/en/latest/ide/atom.html) because I already spend a lot of time learning getting used to jetbrains. 

I want to create an Plugin for jetbrains Clion that integrates with the PlatformIO core for managing 
libraries, development boards and development platforms. The plugin will add several features to Clion like
A new project wizards, new language support, configurable plugin settings, tool windows and project templates.
_Every thing after an **It would be nice** and **Optional** will be added only if there is is enough time available_
The following features will I implement: 
 - An toolbar with buttons to open PlatformIO's library, boards and platform manager.
    - The toolbar contains a button to open de library manager. When pressed an windows needs to be created that allows
        the user to search in the online library repositories.
    - The toolbar contains a button to open de boards manager. When pressed an windows needs to be created that allows
        the user to search in the online board repositories. **It would be nice** if the user is able to choose to switch 
        the project target environment if it is also possible to add an extra target.
    - The toolbar contains a button to open de framework manager. When pressed an windows needs to be created that allows
        the user to search in the online framework repositories. The user should be able to choose to switch the project 
        framework. **It would be nice** If the plugin is able to install new frameworks on the users laptop if it is 
        not currently installed. **It would be nice** if the chosen libraries are automatically included with 
        `#include< lib >` inside the `main.cpp` file.
 - An tool window with access to the PlatformIO commandline tools.
    - The tool window will be accessible through an new toolbar button at the bottom of the page. 
 - An project wizard for creating new PlatformIO project.
    - The wizard should ask the user how to name the project and where to save it. 
    - The wizard should ask the user what target framework and board they want to configure.
    - The wizard should allow the user to select multiple libraries from the online repository that will get downloaded 
      and configured in the platformio configuration file. **It would be nice** to have multiple example projects to choose 
      from, maybe from `examples` folder if the library if available.
 - Language support for the PlatformIO configuration files with syntax highlighting, grammar checking, smart 
   autocompletion and documentation.
 - Integration with the syntax highlighting configuration system.
 - **Optional** Integration with the renaming and refactoring system.
 - **Optional** Integration with the file type and file templates configuration system.
 - **Optional** An serial monitor to communicate with devices.    
 - **Optional** Integration with the structure view panel.
 - **Optional** An option in the file create menu to create an new Arduino project.
 - **Optional** An project wizard for creating new Arduino project.
      - The wizard should allow the user to select multiple libraries from the online repository that will get downloaded 
           and configured in the platformio configuration file. **It would be nice** to have multiple example projects to choose 
           from, maybe from `examples` folder if the library if available. **It would be nice** if the chosen libraries 
           are automatically included with `#include< lib >` inside the `.ino` file.
 - **Optional** Language support for arduino's .ino files with syntax highlighting, grammar checking, smart autocompletion.
 - **Optional** An serial plotter to visualize incoming data from the devices in graphs. 
 - **Optional** Templates for configuration.
 - **Optional** An manager to use the Arduino Library system.
 - **Optional** An manager to import Arduino Libraries.

## Author 
 - Joris Rietveld [jorisrietveld@gmail.com](mailto:jorisrietveld@gmail.com)
 
## Todo
- [x] Write assignment case.
- [ ] Get the assignment case approved by an teacher.
- [ ] Create use cases UML's to determine all the functionality's to implement.
- [ ] Create package diagram UML to get an global overview of all the classes that will need to be created.
- [ ] Create class diagram UML that show what attributes and behaviours of each class haves. 
- [ ] Get the class diagram UML approved by an teacher. 
- [ ] Implementing all classes using [TDD](https://www.youtube.com/watch?v=qmS4ojQ1Pa8) so each behaviour is covered by unit tests.
- [ ] Test each feature inside the Clion IDE to check if it actually works.
    - [ ] Test each feature on  :penguin: Linux.
    - [ ] Test each feature on Windows.
    - [ ] Ask someone to test each feature on mac.
- [ ] Try to get the plugin into the plugin distribution repositories.     

# Changes

# License
Copyright (C) 2017 Joris Rietveld
This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.

