# Tool Learning Log

## Tool: Babylon

## Project: FP

---
## 11/12
#### I used [Babylon](https://www.babylonjs.com/), went to Tools and chose [a playground](https://playground.babylonjs.com/) to tinker with. I wondered what would happen if I change 0.7 of light density of 0.11 because I wasn´t sure of what light density is and after i did that I learned light density is the amount of color in a playground that has only a sphere. I didn't like the shape of the sphere because it was so common so I used this code 

```

// Our built-in 'goldenberg' shape. var sphere = BABYLON.MeshBuilder.CreateGoldberg("Goldenberg", {diameter: 2, segments: 32}, scene); // Move the goldenberg upward 1/2 its height sphere.position.y = 1;

```

#### This code changed the shape of sphere to Goldenberg (name of the shape).

#### To create the shape of Goldenberg because it´s name was just fancy. 

#### In the future, I wish to work with numbers and learn more of new shapes on a sandbox on [Babylon website](https://www.babylonjs.com/) that I don´t know of yet.

### 18/24:
* I went to [Babylon.js website](https://www.babylonjs.com/). I wanted to tinker with height, weight, etc in babylon.

### Before:

```
// Default intensity is 1. Let's dim the light a small amount
    light.intensity = 0.7;

    // Our built-in 'sphere' shape.
    var sphere = BABYLON.MeshBuilder.CreateSphere("sphere", {diameter: 2, segments: 32}, scene);

    // Move the sphere upward 1/2 its height
    sphere.position.y = 1;
```
  ![Screenshot 2024-11-15 11 16 27 AM](https://github.com/user-attachments/assets/2844e9f1-8362-4ce9-9a64-628b8e180f43)

#### I was confused with what `light.density` is, `sphere.position` is, `diameter` & `segments` are so I changed them in order to see what they are.

### After:
This is how I tinker with playground to learn more about positioning and this is after how playground looked like. 

[Screenshot 2024-11-15 11 14 48 AM](https://github.com/user-attachments/assets/6a006926-f853-48c8-860b-d99b6385a82a)

```
 // Default intensity is 1. Let's dim the light a small amount
    light.intensity = 0.5;

    // Our built-in 'sphere' shape.
    var sphere = BABYLON.MeshBui!
lder.CreateSphere("sphere", {diameter: 5, segments: 50}, scene);

    // Move the sphere upward 1/2 its height
    sphere.position.y = 2;
```
#### I learned that `light.density` changed how shape is showen, either dark or light and I increased `light.density`. `Diameter` is width and `segmnet` is like size of the shape or height. `sphere.position` is where the shape is located.

### 11/25/24:

##### I used (websites, videos, etc)

* I used [Babylon's playground feature](https://playground.babylonjs.com/) in order to learn more about diameter and camera position. 

##### My tinkering 

* Since I wanted to learn more about general shapes, variable diameters, I tinkered with them in order to extend my knowledge. 

* These are how I tinkered with code in order to gain more knowledge about diameters, shapes, and positions but I changed sphere to circle. 

###### Diameter and shape of my tinkering 

```JS
<var circle = BABYLON.MeshBuilder.CreateCircle("circle", {diameter: 5, segments: 6}, scene);
```

###### Model Position

```JS
circle.position.y = 5;
```

###### Camera of my shape

```JS
var camera = new BABYLON.FreeCamera("camera1", new BABYLON.Vector3(0, -10, -10), scene);
```


* My tinkering allowed me to change the initial position of my model to the higher ones within the shape to get larger and to become different shape and for me to use parameters to do so

##### What would be my future tinkering 

* Since I completed working with shapes, diameters, light density, positions, etc on Babylon. I would love to work on how to create my own shape with my own functions and variables. 

### 12/2/24:

#### Since I´m done tinkering with playground and it´s all functions. I jump into [https://doc.babylonjs.com/features/introductionToFeatures/chap2/variation/](building a house) and how to tinker with it by understanding it´s code or functions in order to change them to make it my own thing

### Before
```JS
const roof = BABYLON.MeshBuilder.CreateCylinder("roof", {diameter: 2.1, height: 1.2, tessellation: 3});
roof.scaling.x = 0.75;
roof.rotation.z = Math.PI / 2;
roof.position.y = 1.22;
```
#### This piece of code decides position, diameter, height, rotation, and scalling of a adding a roof. However, I tinkered with this roof to make it look and run completely different from the recent one. 

![Screenshot 2024-12-02 11 01 12 AM](https://github.com/user-attachments/assets/96986f8e-06eb-4e2a-b5d5-014603102275)

### After:

#### I added a different type of roof that would make our box more unqiue house like. I kept a same prism like shape which were `cylinder` and `box` which made me to use `CreateCylinder`. Since `cylinder` is like only shape for a roof of house. 
```JS
const box = BABYLON.MeshBuilder.CreateBox("box", {});
    box.position.y = 0.8;
    const roof = BABYLON.MeshBuilder.CreateCylinder("roof", {diameter: 2.2, height: 1.8, tessellation: 3});
    roof.scaling.x = 1.00;
    roof.rotation.z = Math.PI / 2;
    roof.position.y = 2.11;
    const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:5, height:15});
```
![Screenshot 2024-12-02 11 04 01 AM](https://github.com/user-attachments/assets/9c48c2b8-677d-4288-9adc-e345e0023405)

#### Also, I made a unique roof that is completely different from the recent one by changing its scalling, rotation, position, width, height of ground, diamater, heaight, tesselaion of my unique roof, and position of my box which made my roof to look more bigger and a little far away from our box that created my unique roof. Ground got more height than width.

#### There were different levels for this house and I chose challenge 2 by skipping challenge one in order to add a  unique and different Prism Roof Using 'CreateCylinder'. Therefore, my next challenge in order to complete this house would be challenge 4 because I want to challenge myself more. 
<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
