# Functions for the module Robotik
## Get Started:
1. [Download](https://github.com/samy4sam/ti-nspire/raw/master/Robotic/robotic.tns) the robotic.tns file.
2. Open the robotic.tns file with the TI-Nspire™ CX CAS Student Software.
3. Connect your TI-Nspire™ CX CAS over the USB cable with your PC.
4. In the software go to File/Save to Handheld...
5. Double click on your TI-Nspire™ CX CAS in the appeared window. 
6. Go to "MyLib", rename the file to "robotic" and press Save.
7. Open a new Calculator page on your TI-Nspire™ CX CAS.
8. Press the "doc" button.
9. Update the libraries by pressing the number 6.
10. To access the new functions, press the library button, the number 6 and search for "robotic".
***
## Functions:
### robotic/atan2(y,x)
Function to calculate the arctan2. See [Wikipedia](https://de.wikipedia.org/wiki/Arctan2)  

Parameters:  
* y: sinus  
* x: cosinus  

Returns: 
* Related angle θ  

Note: works for rad and deg. Calculater settings are crucial.  

### robotic/rotx(θ)
Function to get the rotation matrix around the x-axis.  

Parameters:  
*  θ [rad]: Angle around the x-axis.  

Returns: 
* rotation matrix (4x4).

### robotic/roty(θ)
Function to get the rotation matrix around the y-axis.  

Parameters:  
*  θ [rad]: Angle around the y-axis.  

Returns: 
* rotation matrix (4x4).

### robotic/rotz(θ)
Function to get the rotation matrix around the z-axis.  

Parameters:  
*  θ [rad]: Angle around the z-axis. 

Returns: 
* rotation matrix (4x4).

### robotic/xyzangles(r)
Function to calculate the retransformation according to the X-Y-Z Roll-Gier-Nick Convention.

Parameters:
* r (3x3): Rotation matrix. 

Returns: 
* β [rad]
* α [rad]
* γ[rad]

### robotic/zyzangles(r)
Function to calculate the retransformation according to the Z-Y-Z Euler Convention.

Parameters:  
* r (3x3): Rotation matrix. 

Returns:   
* β [rad] 
* α [rad] 
* γ[rad]

### robotic/jacobi(xe,ye,Φe,θ1,θ3,d2)
Function to calculate the Jacobi matrix. The Jacobi matrix of a robot arm describes the mapping of joint velocities to the linear velocity of the TCP and the temporal changes of the orientation of the end-effector.  

Parameters:
* xe: Position in X-direction of the TCP.
* ye: Position in Y-direction of the TCP.
* Φe: Angle of the TCP.
* θ1: Angle of the first section of the robot.
* θ3: Angle of the last section of the robot.
* d2: Lenght of the first section of the robot.
<image src="https://github.com/samy4sam/ti-nspire/blob/master/Robotic/Photos/jacobiMatrix.PNG?raw=true" height=500 />

Returns:
* Jacobi matrix


