# Download Code and Unzip
This step is unecessary if the code is already on the computer, you can check it by looking for the folder Mario-java-main, if it is not there, download the zip folder above, by clicking code and download zip. Open the folder in file explorer and it should automatically open 7-zip, when it does this click the folder and hit extract.
# Opening The Game
In order to modify the code and run it at all, open Visual Studio Code on you laptop, and if necessary, hit open folder and then select Mario-java-main. This should open all of the code for the project.
# Changing the running speed and jump height of Mario
Changing the running speed and jump height of Mario is pretty simple, in order to change the jump height of Mario go to the model folder, and then open the hero folder, and open the Mario class. On lines 60 through 67 change the values of  setVelX(5); and   setVelX(-5); to change the speed Mario runs in those directions. And in order to change Mario's jump height go to line 54 and change the value of setVelY(12);
# Adding another map
In order to add a map go to the view folder and then open the MapSelection File. And on line 45 add the line of code maps.add("Map 3.png"); 
# Changing The Title Screen
If we put Mr.Dockett in the game then it is no longer Super Mario Bros. so first thing we need to do is change the title screen. Open UIManager in the view folder. And on line 37 simply change the value inside of  this.startScreenImage = loader.loadImage("/start-screen.png"); to this.startScreenImage = loader.loadImage("/dockett-screen.png");
# Changing Mario
Changing Mario is almost identical to changing the title screen. Go to the ImageLoader in the view folder and go to line 15. Change mario-forms in the parentheses. To docket forms. This will make Mario Mr.Dockett.
# Changing Jump
Mr.Dockett doesn't like jumping, so in order to do it less often, we'll make the jump a dedicated button. In order to do this go to the manager folder, and then open the Input Manager class. Delete the else statement on line 25 through 27. And then on line 38 put in this statement  
if (keyCode == KeyEvent.VK_SPACE) {
                currentAction = ButtonAction.JUMP;
                }

