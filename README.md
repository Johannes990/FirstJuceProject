Here is my first attempt to create an audio plugin from scratch in cpp using JUCE, instead of using NI Reaktor.

Made during school winter break, using this video as a guide: https://www.youtube.com/watch?v=i_Iq4_Kd7Rc&t=14397s&ab_channel=freeCodeCamp.org

The audio part works fine, but the spectrum analyzer implementation (which uses code from a paid course, and is not covered very well in the guide video at all)
isn't working. Didn't have time to fix it either, because school started again...

To run:
* Clone JUCE repository: https://github.com/juce-framework/JUCE
* From where ever you installed JUCE, open: JUCE/extras/Projucer/Builds and got to your OP/system folder. I'm running Win10, so I used Builds/VisualStudio2022
* Open the solution file (Projucer.sln in Win10, for example)
* Build the solution file in your IDE.
* Open the build folder and locate Projucer. I'm using Visualstudio 2022, so for me: Builds/VisualStudio2022/x64/Debug/App/Projucer.exe
* Set up your global paths in Projucer in File -> Global Paths. However by default these should already be set up to your users folder.
* Select File -> New Project -> Plug-In -> Basic
* Name it FirstJuceProject
* Select Create Project... and save it to a location of your choosing
* Copy files PluginEditor.h, PluginEditor.cpp, PluginProcessor.h and PluginProcessor.cpp to Source folder in your new project
* Open the jucer file in your project folder -> select Modules on the left pane -> click on the plus icon at the bottom -> Add a module -> Global JUCE modules path -> juce_dsp
* Click on Save and Open in IDE
* Run build on either Standalone or VST

:)
