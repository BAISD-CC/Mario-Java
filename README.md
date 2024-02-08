# Step 1: Download Code and Unzip
This step is unecessary if the code is already on the computer, you can check it by looking for the folder Mario-java-main, if it is not there, download the zip folder above, by clicking code and download zip. Open the folder in file explorer and it should automatically open 7-zip, when it does this click the folder then click extract.

# Step 2: Opening The Game
In order to modify the code and run it at all, open Visual Studio Code on you laptop, and if necessary, click open folder and then select Mario-java-main. This should open all of the code for the project.

# Step 3: Changing the running speed and jump height of Mario
Changing the running speed and jump height of Mario is pretty simple, in order to change the jump height of Mario go to the model folder, and then open the hero folder, and open the Mario class. 

On lines 65 and 70 change the values of  setVelX(5); and setVelX(-5); to change the speed Mario runs in those directions. 

To change Mario's jump height go to line 55 and change the value of setVelY(12);

# Step 4: Changing Goomba Speed
In order to change the enemy speed go to the model folder, open the enemy folder and then open the Goomba file. On line 14 change the value of setVelX(3); to whatever you would like.

# Step 5: Adding another map
In order to add a map go to the view folder and then open the MapSelection File. And on line 45 add the line of code maps.add("Map 3.png"); 

# Step 6: Changing The Title Screen
If we put Mr.Kruskie in the game then it is no longer Super Mario Bros. so first thing we need to do is change the title screen. Open UIManager in the view folder. 

On line 37 simply change the value inside of  this.startScreenImage = loader.loadImage("/start-screen.png"); to this.startScreenImage = loader.loadImage("/kruskie-screen.png");

# Step 7: Changing Mario
Changing Mario is almost identical to changing the title screen. Go to the ImageLoader in the view folder and go to line 15. Change mario-forms in the parentheses. To kruskie-forms. This will make Mario Mr. Kruskie.

# Step 8: Changing Jump
Mr.Kruskie doesn't like jumping, so in order to do it less often, we'll make the jump a dedicated button. In order to do this go to the manager folder, and then open the Input Manager class. On line 30 put the following:
if (keyCode == KeyEvent.VK_SPACE) {
            currentAction = ButtonAction.JUMP;
        }

