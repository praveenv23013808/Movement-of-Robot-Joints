#8,Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)
```
## Output
### 1. Generic Articulated Robot
![281066215-31417441-9576-4a78-a04a-ebcce4902dfc](https://github.com/praveenv23013808/Movement-of-Robot-Joints/assets/145824728/716ac13f-e232-42dd-b321-bc98a875de4f)
### 2. robot.driveJoints(0,0,0,0,0,0)
![281066565-ce203c1f-da82-4d9e-aa80-8c43dd82df81](https://github.com/praveenv23013808/Movement-of-Robot-Joints/assets/145824728/1f38a096-b07e-4851-b34d-33b9f1dff247)
### 3. Movement of Joint1
![281066460-262b9fde-874c-49c9-8daa-dfc53a509a81](https://github.com/praveenv23013808/Movement-of-Robot-Joints/assets/145824728/f774a1af-0dd0-4878-b790-deb1c772247c)
### 3. Movement of Joint2
![281066525-c099b932-bf3b-4df3-9ec3-f3c9d28799f4](https://github.com/praveenv23013808/Movement-of-Robot-Joints/assets/145824728/9c788f11-f49d-4b5b-a129-3ed6bc447152)
### 3. Movement of Joint3
![281066565-ce203c1f-da82-4d9e-aa80-8c43dd82df81](https://github.com/praveenv23013808/Movement-of-Robot-Joints/assets/145824728/1f38a096-b07e-4851-b34d-33b9f1dff247)
## Result 
Thus the different robots joints are moved with the help of python list.


