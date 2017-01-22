Three.js Geometry Editor
------------------------

## Summary
This is a visual three dimensional plane editor for three.JS.  You can customize a size plane and easily edit each individual vertice and export the code.

[Try it out](https://tylario.github.io/Threejs-geometry-editor/)

## Usage
To begin select a size using the Length & height button. Ex: 10 by 15, 2 by 4, 8 by 8

Next click set and confirm to create the plane.

You will see a red dot over the selected vertice

To select a different vertice use the arrow keys (left, right, up & down)

To position the vertice use WASD  
* W is up
* S is down
* A is left (either on X axis or Z axis)
* D ir right (either on X axis or Z axis)

To rotate the plane press space - this will also allow you to edit the position of the vertice on the Z axis instead of the X axis

Once you are finished with the plane click ***get code***, this will give you the code for the plane, which you can copy and paste into your own code


## Code Example
```
var geometry = new THREE.PlaneGeometry(_length_, _height_, _numVerticesHoriz_, _numVerticesVertical_);

/* insert exported code here */

var material = new THREE.MeshPhongMaterial({ color: 0x000, wireframe: true });

var mesh = new THREE.Mesh(geometry, material);
scene.add(mesh);
```
