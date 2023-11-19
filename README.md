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
<img width="754" alt="Screenshot 2023-11-19 at 10 05 57 AM" src="https://github.com/Murthy46/Movement-of-Robot-Joints/assets/145112768/26c498b7-330a-4082-aff2-341e0443123a">

</br>
</br>
</br>
</br>

### 2. robot.driveJoints(0,0,0,0,0,0)
<img width="749" alt="Screenshot 2023-11-19 at 10 06 12 AM" src="https://github.com/Murthy46/Movement-of-Robot-Joints/assets/145112768/2e6269aa-e2f7-43fe-b0a3-6ae2da315905">

</br>
</br>
</br>
</br>

### 3. Movement of Joint1
<img width="755" alt="Screenshot 2023-11-19 at 10 06 34 AM" src="https://github.com/Murthy46/Movement-of-Robot-Joints/assets/145112768/fa1d4c4c-d8c3-4d14-89eb-80d8740c30e0">

</br>
</br>
</br>
</br>

### 3. Movement of Joint2
<img width="756" alt="Screenshot 2023-11-19 at 10 06 51 AM" src="https://github.com/Murthy46/Movement-of-Robot-Joints/assets/145112768/13af4b75-db93-4ac0-972a-1d02eba32786">

</br>
</br>
</br>
</br>

### 3. Movement of Joint3
<img width="758" alt="Screenshot 2023-11-19 at 10 07 08 AM" src="https://github.com/Murthy46/Movement-of-Robot-Joints/assets/145112768/e36d1738-2a06-45c2-9ca6-2eeae0ac3aa4">

</br>
</br>
</br>
</br>

## Result 
Thus the different robots joints are moved with the help of python list.


