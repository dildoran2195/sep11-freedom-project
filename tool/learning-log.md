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

#### Since I´m done tinkering with playground and it´s all functions. I jump into [building a house](https://doc.babylonjs.com/features/introductionToFeatures/chap2/variation/) and how to tinker with it by understanding it´s code or functions in order to change them to make it my own thing

### Before
```JS
const roof = BABYLON.MeshBuilder.CreateCylinder("roof", {diameter: 2.1, height: 1.2, tessellation: 3});
roof.scaling.x = 0.75;
roof.rotation.z = Math.PI / 2;
roof.position.y = 1.22;
```
#### This piece of code decides position, diameter, height, rotation, and scalling of a adding a roof. However, I tinkered with this roof to make it look and run completely different from the recent one. I was confused with what tesselation is and why it is important for a roof of my house. 

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

#### Also, I made a unique roof that is completely different from the recent one by changing its scalling, rotation, position, width, height of ground, diamater, heaight, tesselaion of my unique roof, and position of my box which made my roof to look more bigger and a little far away from our box that created my unique roof. Ground got more longer through it´s new height than it´s old width.

#### There were different levels for this house and I chose challenge 2 by skipping challenge one in order to add a  unique and different Prism Roof Using 'CreateCylinder'. Therefore, my next challenge in order to complete this house would be challenge 4 because I want to challenge myself more. 

#### my a-ha moment was what tesselation is and why it´s important. Therefore I changed my tesselation from 2 to 5 to know what it does and why it is important.
![Screenshot 2024-12-02 11 17 37 AM](https://github.com/user-attachments/assets/42d1549a-cf81-4a6a-9dbe-ee10682acf70)
#### I learned that tesselation is like shape of a roof that changed how it looks like

### 01/02/25

### My resources and goal:

#### I wanted to continue on building a house which was tinkering with world objects in order to learn about certain functions that I am not familar with. I used [Add Texture](https://doc.babylonjs.com/features/introductionToFeatures/chap2/material/) as resource of mine. I also went to [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

### Before:
![Screenshot 2024-12-20 10 46 54 AM](https://github.com/user-attachments/assets/51457ed7-cfa2-4b6b-95d0-5c1d34bc66d6)
```
    /**** World Objects *****/
    const box = BABYLON.MeshBuilder.CreateBox("box", {});
    box.material = boxMat;
    box.position.y = 0.5;
    const roof = BABYLON.MeshBuilder.CreateCylinder("roof", {diameter: 1.3, height: 1.2, tessellation: 3});
    roof.material = roofMat;
    roof.scaling.x = 0.75;
    roof.rotation.z = Math.PI / 2;
    roof.position.y = 1.22;
    const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:10, height:10});
    ground.material = groundMat;

    return scene;
}
```
```
    //color
    const groundMat = new BABYLON.StandardMaterial("groundMat");
    groundMat.diffuseColor = new BABYLON.Color3(0, 1, 0)
```
### Things you tried, tinkered with, your progress, etc.,:

#### I was confused about certain functions of this house including what  `roof.material = roofMat;` , `roof.scaling.x = 0.75;` , `roof.rotation.z = Math.PI / 2;` , `roof.position.y = 1.22;` , and  `const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:10, height:10});`. Therefore, I tinker with these functions to learn what its purpose is and what is does.

### After:
![Screenshot 2024-12-16 11 14 59 AM](https://github.com/user-attachments/assets/fbab55bb-0b71-43f8-bb85-4833bad92528)
```
    /**** World Objects *****/
    const box = BABYLON.MeshBuilder.CreateBox("box", {});
    box.material = boxMat;
    box.position.y = 0.20;
    const roof = BABYLON.MeshBuilder.CreateCylinder("roof", {diameter: 2.3, height: 2.2, tessellation: 4});
    roof.material = roofMat;
    roof.scaling.x = 0.55;
    roof.rotation.z = Math.PI / 2;
    roof.position.y = 1.30;
    const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:12, height:12});
    ground.material = groundMat;
```
```
    /**** Materials *****/
    //color
    const groundMat = new BABYLON.StandardMaterial("groundMat");
    groundMat.diffuseColor = new BABYLON.Color3(0.96, 0.07, 0.96)
```
### Things you learned through tinkering:

#### I learned purpose of  `roof.material = roofMat;` was texture of this house, `roof.scaling.x = 0.75;` was size of the roof, `roof.rotation.z = Math.PI / 2;` rotates the roof , `roof.position.y = 1.22;`  changes size or position of the roof, and  `const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:10, height:10});` is how big and how long the ground is.

### a-ha moments or challenge:

#### I was able to create a different model types using Babylon in order to build a house. I was also able to use different properties to maneuver models.

### Questions I still have
#### How to implement animations using challenge of making a house.

### What you're going to try next:

#### My next step is to tinker with [Material For Each House Side](https://doc.babylonjs.com/features/introductionToFeatures/chap2/face_material/) which is basically adding door and multiple windows for this house using Babylon.

## 01/13/25
### My resources and goal:
#### MY goal was to tinker with [Material For Each House Side](https://doc.babylonjs.com/features/introductionToFeatures/chap2/face_material/) which is basically building materials to the house and how house looks like in outside. I also to [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

### Before:
![Screenshot 2025-01-06 2 21 15 PM](https://github.com/user-attachments/assets/9334a344-5c29-4805-a5b9-1a3523a5b7d5)
![Screenshot 2025-01-06 2 18 33 PM](https://github.com/user-attachments/assets/d852416f-40a4-41c8-af81-22fcb462dd8f)
```
    /**** Set camera and light *****/
    const camera = new BABYLON.ArcRotateCamera("camera", -Math.PI / 2, Math.PI / 2.5, 10, new BABYLON.Vector3(0, 0, 0));
    camera.attachControl(canvas, true);
    const light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(1, 1, 0));

    /**** Materials *****/
    //color
    const groundMat = new BABYLON.StandardMaterial("groundMat");
    groundMat.diffuseColor = new BABYLON.Color3(0, 1, 0)

    //texture
    const roofMat = new BABYLON.StandardMaterial("roofMat");
    roofMat.diffuseTexture = new BABYLON.Texture("https://assets.babylonjs.com/environments/roof.jpg");
    const boxMat = new BABYLON.StandardMaterial("boxMat");
    boxMat.diffuseTexture = new BABYLON.Texture("https://assets.babylonjs.com/environments/cubehouse.png")


    //options parameter to set different images on each side
    const faceUV = [];
    faceUV[0] = new BABYLON.Vector4(0.5, 0.0, 0.75, 1.0); 
    faceUV[1] = new BABYLON.Vector4(0.0, 0.0, 0.25, 1.0);
    faceUV[2] = new BABYLON.Vector4(0.25, 0, 0.5, 1.0); 
    faceUV[3] = new BABYLON.Vector4(0.75, 0, 1.0, 1.0); 
    // top 4 and bottom 5 not seen so not set
```

### Things you tried, tinkered with, your progress, etc.,:
I was confused with purpose of certain codes including `const camera`, `const light`, `const groundMat` and `const faceUV = [];` which had plenty of codes inside. All of these certain codes are materiuals of texture, color, and options parameter to set different images on each side which I've tinkered with so far.
### After:
![Screenshot 2025-01-06 2 16 54 PM](https://github.com/user-attachments/assets/4b9b1771-9dce-473c-8ccb-405bcb6febf9)
![Screenshot 2025-01-06 2 17 27 PM](https://github.com/user-attachments/assets/e7afb6a6-6c08-4dd7-b5c9-c97d16153966)
```
    /**** Set camera and light *****/
    const camera = new BABYLON.ArcRotateCamera("camera", -Math.PI / 4, Math.PI / 3.8, 12, new BABYLON.Vector3(1, 2, 3));
    camera.attachControl(canvas, true);
    const light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(1, 1, 1));

    /**** Materials *****/
    //color
    const groundMat = new BABYLON.StandardMaterial("groundMat");
    groundMat.diffuseColor = new BABYLON.Color3(0.07, 0.09, 0.93)

    //texture
    const roofMat = new BABYLON.StandardMaterial("roofMat");
    roofMat.diffuseTexture = new BABYLON.Texture("https://assets.babylonjs.com/environments/roof.jpg");
    const boxMat = new BABYLON.StandardMaterial("boxMat");
    boxMat.diffuseTexture = new BABYLON.Texture("https://assets.babylonjs.com/environments/cubehouse.png")


    //options parameter to set different images on each side
    const faceUV = [];
    faceUV[0] = new BABYLON.Vector4(1, 1, 0.85, 1.0); 
    faceUV[1] = new BABYLON.Vector4(0.5, 0.10, 0.15, 1.5); 
    faceUV[2] = new BABYLON.Vector4(0.29, 1, 1.5, 1.5); 
    faceUV[3] = new BABYLON.Vector4(0.85, 1, 1.5, 1.5); 
    // top 4 and bottom 5 not seen so not set
```

### Things you learned through tinkering:
#### I learned that  `const camera` is how the house is seen all the way from top so it's like a camera that shows how house actually looks like, `const light` is how light or how dark the house is, `const groundMat` and `const faceUV = [];` which had plenty of codes inside.
### a-ha moments or challenge:

### Questions I still have:

### What you're going to try next:

<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
