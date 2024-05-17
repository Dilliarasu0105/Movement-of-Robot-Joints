# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
Developed by: Dilliarasu M
RegisterNumber: 212223230049
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)





```
## Output
### 1. Generic Articulated Robot

![image](https://github.com/Dilliarasu0105/Movement-of-Robot-Joints/assets/144979593/c6496b5a-9378-410b-90f9-86425a54a674)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/Dilliarasu0105/Movement-of-Robot-Joints/assets/144979593/3e9d3479-23af-404b-b8f1-93273e7a3657)


### 3. Movement of Joint1
![image](https://github.com/Dilliarasu0105/Movement-of-Robot-Joints/assets/144979593/9a8f0c5c-63d4-4eee-9ef5-90d31adcb914)


### 4. Movement of Joint2
![image](https://github.com/Dilliarasu0105/Movement-of-Robot-Joints/assets/144979593/49d6a3b5-3945-4681-b4cf-6e72ff08b6d8)


### 5. Movement of Joint3
![image](https://github.com/Dilliarasu0105/Movement-of-Robot-Joints/assets/144979593/9e807ac1-08ed-4896-b068-12a3a11773c8)


## Result 
Thus the different robots joints are moved with the help of python list.


