#  Trackpad setup toggle script

## :confused: Summary
* Applescript to quickly toggle my custom trackpad settings on/off.
* Prevents frustration in others who use my machine.

## :mouse: My trackpad setup
* Correct scrolling. (Default is backwards.)
* Three Finger Drag. (Default is off.)
* Four finger up swipe for Mission Control. (Default is 3; can't coexist with three finger drag.)

## :question: Why?
 * **Drag:** On my first mac, my trackpad's button broke. To click anything, I had to enable tap-to-click. To move anything, I had to enable three finger drag. Out of necessity I saw the light: these settings are more efficient.
 * **Scroll direction:** In 2011 Apple released OS X Lion, flipping the default direction of two finger scroll. I've been using macs since before 2011. (Is there a hipster emoji?)

## :shipit: To install
* Pull repo
* Open the Applescript with Script Editor
* Read "Gotchas" section.
* Click run or press <code>command r</code>
* Bonus:
  * Export Applescript as an Application. (Script Editor -> File -> Export...)
  * Then, either put the Application in your dock, or memorize whatever you name it, so you can spotlight-run it quickly.


## :heavy_exclamation_mark: Gotchas
* You must authorize control of your computer.
### Won't run properly in Applescript Editor
* System Preferences -> Security & Privacy -> Accessibility -> Add 'Script Editor' to 'Allow the apps below to control your computer.
### Exported Application won't run properly.
* System Preferences -> Security & Privacy -> Accessibility -> Add '[Exported App]' to 'Allow the apps below to control your computer.'


## :arrow_up_down: I only want to toggle scroll direction.

* No problem!  
  * Pull this repo
  * Open the Applescript with Script Editor
  * Find the following line: <code>set shouldAlsoToggleThreeFingerDrag to true</code> (
  * Change <code>true</code> to <code>false</code>
