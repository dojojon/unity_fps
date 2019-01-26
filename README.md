# DOJO Note for Unity FPS

**NOTE: This is not a full unity project with scenes and assets, but notes and example scrips**

The scrips and steps are based on tutorials from Wireframe Magazine.  https://wireframe.raspberrypi.org/issues

Issue 3, Issue 5

## Scripts


## Steps for Issue 3

The following steps broadly follow the Issue 3 artcle, but with lots fo details missed out.

### Adding a ```Player```

1. Install Unity - https://unity3d.com/get-unity/download
2. Create new project, select template 3d.
3. Add ```Player```
    1. Add a 3d object of type capsule
    2. Rename to ```Player```
    3. Move ```Main Camera``` into ```Player```
    4. Reset position ```Main Camera``` so it sits inside player    
    5. Set ```Main Camera``` to be higher so it simulats players eyes in head
4. Add ```Player``` base movement script
    1. In Project window add a ```Scripts``` directory in ```Assets```
    2. Add a script and name it ```PlayerMovement```.  ** Unity expects the class name and file name to match or it goes wonky **
    3. Double click to open in Visual Studio
    4. Copy the example ```PlayerMovement``` code into this new file
    5. Save the script in Visual Studio
    6. In Unity drag the script onto the ```Player``` Capsule
    7. Note the component in the inspector view for the  ```Player``` object.
5. Click the play button, escape to exit
6. Add ```Ground```
    1. Add a 3d object of type plane
    2. Rename it to ```Ground```
    3. Move it down by changing the Y in inspector
    3. Make it bigger by changing the X and Y scale in inspector (10 for now)
7. Click the play button, escape to exit
8. Fixing jump
    1. Add RigidBody component to the ```Player```
9. Click the play button, escape to exit
    1. Try jumping and turning at the same time.
    2. Player may fall over.
10. Fix falling over
    1. In inspector, got to the Rigid Body component, Constraints.
    2. Check the ```Freeze Rotation``` x and z
11. Click the play button, escape to exit
    1. Try jumping and turning at the same time.
    2. Player may fall over.    

### Adding a ```Cube``` to look at

1. Add a Cube of type Cube
2. Rename in ```Wall```
2. Select the scene view 
3. Use the Gizmo arrows to drag it around
4. Use inspector to change the scale and fine tune its possition
    1. Scale 10, 4, 1
    2. Position 0, 1, 6
5. In Project window add a ```Materials``` directory in ```Assets```
6. Add new material in here, name it something appropriate ```BlueWall```
7. Set the materials color.
8. Drag material onto wall
7. Click the play button, escape to exit
    1. Notice we can't look around using the mouse.

### Add looking around

1. In the scrpts folder add a new script
2. Name it ```MouseLook```
3. Double click to open in Visual Studio
    4. Copy the example ```MouseLook``` code into this new file
    5. Save the script in Visual Studio
    6. In Unity drag the script onto the ```Camera``` Capsule
7. Click the play button, escape to exit
    1. Notice we can't look around using the mouse.


