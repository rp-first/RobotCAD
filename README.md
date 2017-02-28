RobotCAD
========

This project is a simple example of how to create a Unity App for the Microsoft
HoloLens that allows for the display of an FRC robot CAD drawing as a hologram.
This allows the HoloLens wearer to walk through the robot and examine the
components in detail.

Process summary:
================

1.  Simplify your CAD drawing

2.  Export the CAD to OBJ or FBX if possible.

3.  If not, export to STL and then use something like MeshLab or Autodesk
    Meshmixer to convert it to OBJ. You may also need to reduce the size of the
    mesh.

4.  Build a new Unity project, import the HoloToolKit

5.  Import the robot and setup TapToPlace or other features you would like to
    use.

6.  Build and deploy to the Hololens.

Please refer to the detail walkthrough described in the RobotCAD.md file under
the docs folder.

The CAD drawing in this project is for FRC Team 330 The Beach Bots’ 2016
“Stronghold” robot (after several reductions so it was small enough to upload to
Github). You can replace it with the CAD drawing from your team by importing it
as a new asset and replacing the robot child object in the RobotBase object in
the project. Then adjust the scale size and add a Mesh Renderer component. See
the RobotCAD.md in the docs folder for details.
