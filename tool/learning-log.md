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

#### I wanted to continue building a house which was tinkering with world objects in order to learn about certain functions that I am not familiar with. I used [Add Texture](https://doc.babylonjs.com/features/introductionToFeatures/chap2/material/) as a resource of mine. I also went to [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

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

#### I was confused about certain functions of this house including what  `roof.material = roofMat;` , `roof.scaling.x = 0.75;` , `roof.rotation.z = Math.PI / 2;` , `roof.position.y = 1.22;` , and  `const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:10, height:10});`. Therefore, I tinker with these functions to learn what its purpose is and what it does.

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

#### I was able to create different model types using Babylon in order to build a house. I was also able to use different properties to maneuver models.

### Questions I still have
#### How to implement animations using the challenge of making a house.

### What you're going to try next:

#### My next step is to tinker with [Material For Each House Side](https://doc.babylonjs.com/features/introductionToFeatures/chap2/face_material/) which is basically adding doors and multiple windows for this house using Babylon.

## 01/13/25
### My resources and goal:
#### My goal was to tinker with [Material For Each House Side](https://doc.babylonjs.com/features/introductionToFeatures/chap2/face_material/) which is basically building materials to a house and how a house looks like in outside. I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

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
I was confused with the purpose of certain codes including 'const camera`, `const light`, `const groundMat` and `const faceUV = [];` which had plenty of codes inside. All of these certain codes are materials of texture, color, and options parameter to set different images on each side which I've tinkered with so far.
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
#### I learned that  `const camera` is how a house is seen all the way from top so it's like a camera that shows how a house actually looks like, `const light` is how light or how dark a house is, `const groundMat` is size (height/weight) of ground and `const faceUV = [];` which had plenty of codes inside are rear face, front face, right side, and left side of a house.
    
### a-ha moments or challenge:
#### I was able to create different model types using Babylon in order to make the materials of a house. I was also able to use different properties to maneuver models in order to tinker with materials of a house.
### Questions I still have:
#### How to implement more animations using the challenge of making a house.
### What you're going to try next:
#### I'm going to try [Expanding the House Building Function](https://playground.babylonjs.com/#KBS9I5#77)

### 3.4.25
## 01/13/25
### My resources and goal:
#### My goal was to tinker with 3D objects [copying meshes](https://playground.babylonjs.com/#KBS9I5#78) which is basically making copy of 3D objects to a house and how a house looks like in outside. I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

### Before:
![Screenshot 2025-02-28 3 24 18 PM](https://github.com/user-attachments/assets/5fc11333-d72f-4d1c-8ecd-20b7aeb80a57)

```
/******Build Functions***********/
const buildGround = () => {
    //color
    const groundMat = new BABYLON.StandardMaterial("groundMat");
    groundMat.diffuseColor = new BABYLON.Color3(0, 1, 0);

    const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:15, height:16});
    ground.material = groundMat;
}
places.push([1, -Math.PI / 16, -6.8, 2.5 ]);
    places.push([2, -Math.PI / 16, -4.5, 3 ]);
    places.push([2, -Math.PI / 16, -1.5, 4 ]);
    places.push([2, -Math.PI / 3, 1.5, 6 ]);
    places.push([2, 15 * Math.PI / 16, -6.4, -1.5 ]);
    places.push([1, 15 * Math.PI / 16, -4.1, -1 ]);
    places.push([2, 15 * Math.PI / 16, -2.1, -0.5 ]);
    places.push([1, 5 * Math.PI / 4, 0, -1 ]);
    places.push([1, Math.PI + Math.PI / 2.5, 0.5, -3 ]);
    places.push([2, Math.PI + Math.PI / 2.1, 0.75, -5 ]);
    places.push([1, Math.PI + Math.PI / 2.25, 0.75, -7 ]);
    places.push([2, Math.PI / 1.9, 4.75, -1 ]);
    places.push([1, Math.PI / 1.95, 4.5, -3 ]);
    places.push([2, Math.PI / 1.9, 4.75, -5 ]);
    places.push([1, Math.PI / 1.9, 4.75, -7 ]);
    places.push([2, -Math.PI / 3, 5.25, 2 ]);
    places.push([1, -Math.PI / 3, 6, 4 ]);

const faceUV = [];
    if (width == 2) {
        faceUV[0] = new BABYLON.Vector4(0.6, 0.0, 1.0, 1.0); //rear face
        faceUV[1] = new BABYLON.Vector4(0.0, 0.0, 0.4, 1.0); //front face
        faceUV[2] = new BABYLON.Vector4(0.4, 0, 0.6, 1.0); //right side
        faceUV[3] = new BABYLON.Vector4(0.4, 0, 0.6, 1.0); //left side
    }
    else {
        faceUV[0] = new BABYLON.Vector4(0.5, 0.0, 0.75, 1.0); //rear face
        faceUV[1] = new BABYLON.Vector4(0.0, 0.0, 0.25, 1.0); //front face
        faceUV[2] = new BABYLON.Vector4(0.25, 0, 0.5, 1.0); //right side
        faceUV[3] = new BABYLON.Vector4(0.75, 0, 1.0, 1.0); //left side
    }
```

### Things you tried, tinkered with, your progress, etc.,:
I was confused with the purpose of certain codes including 'const camera`, faceUV[0]`, `const groundMat` and `places.push([1, -Math.PI / 16, -6.8, 2.5 ]);` which had plenty of codes inside. All of these certain codes are materials of an array, position, rotation, apperance, side length, width, height, house type, rotation, and x, z which I've tinkered with so far.
### After:
![Screenshot 2025-02-28 3 49 13 PM](https://github.com/user-attachments/assets/33611f5d-6458-47aa-bca3-5580cb8bf1e8)
![Screenshot 2025-02-28 3 49 27 PM](https://github.com/user-attachments/assets/cc76c932-6967-46d6-8a5b-81ff558ab942)

```
places.push([1, -Math.PI / 19, -6.8, 2.5 ]);
    places.push([2, -Math.PI / 18, -9.5, 8 ]);
    places.push([2, -Math.PI / 19, -1.9, 7 ]);
    places.push([2, -Math.PI / 6, 9.5, 5 ]);
    places.push([2, 15 * Math.PI / 19, -6.4, -1.5 ]);
    places.push([1, 15 * Math.PI / 18, -4.1, -1 ]);
    places.push([2, 15 * Math.PI / 19, -2.1, -0.5 ]);
    places.push([1, 5 * Math.PI / 2, 0, -1 ]);
    places.push([1, Math.PI + Math.PI / 3.5, 0.5, -3 ]);
    places.push([2, Math.PI + Math.PI / 2.1, 0.75, -5 ]);
    places.push([1, Math.PI + Math.PI / 2.25, 0.75, -7 ]);
    places.push([2, Math.PI / 6.9, 6.75, -1 ]);
    places.push([1, Math.PI / 5.95, 8.5, -3 ]);
    places.push([2, Math.PI / 5.9, 4.75, -5 ]);
    places.push([1, Math.PI / 6.9, 8.75, -7 ]);
    places.push([2, -Math.PI / 6, 5.25, 44 ]);
    places.push([1, -Math.PI / 6, 7, 8 ]);

const faceUV = [];
    if (width == 2) {
        faceUV[0] = new BABYLON.Vector4(5.1, 6.0, 5.0, 2.0); //rear face
        faceUV[1] = new BABYLON.Vector4(5.9, 5.0, 5.4, 5.0); //front face
        faceUV[2] = new BABYLON.Vector4(9.4, 4, 2.6, 4.0); //right side
        faceUV[3] = new BABYLON.Vector4(3.4, 2, 7.6, 4.0); //left side
    }
    else {
        faceUV[0] = new BABYLON.Vector4(3.9, 3.5, 1.75, 2.0); //rear face
        faceUV[1] = new BABYLON.Vector4(4.9, 2.6, 1.25, 2.0); //front face
        faceUV[2] = new BABYLON.Vector4(5.25, 2, 8.5, 5.0); //right side
        faceUV[3] = new BABYLON.Vector4(6.75, 4, 1.0, 2.0); //left side

const box = BABYLON.MeshBuilder.CreateBox("box", {width: width, faceUV: faceUV, wrap: true});
    box.material = boxMat;
    box.position.y = 0.5;
    box.position = 9.9
    box.getFacetDataParameters = 10
    box.scaling = 9
    return box;
}
const buildGround = () => {
    //color
    const groundMat = new BABYLON.StandardMaterial("groundMat");
    groundMat.diffuseColor = new BABYLON.Color3(0, 1, 0);

    const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:30, height:29});
    ground.material = groundMat;
}

```

### Things you learned through tinkering:
#### I learned that `const places = [];` represents each entry that is an array of house type, rotation, and x, z. I learned how to make 3D objects, shapes, how to change its functions, and how to make multiple of them at the same time using advanced Babylon. However, I mainly tinkered with its parameters, 3D shapes, height, world objects, texture, colors, array, width, material, scaling, rotation, x, y, positions, camera & light, and how to create instances from the first two that were built. I learned that `const faceUV = [];` is a parameter that gives multiple options to set different images on each side of the house. Also, I was confused with what functions of `faceUV = [];` represent, like which one represents which house but I was able to figure it out by tinkering so I saw their purpose, `faceUV[0]` --> rear face, `faceUV[1]`--> `front face`, `faceUV[2]`--> right side, and `faceUV[3]`--> left side. Below is my tinkerings: Below are my tinkerings from top to bottom of my result:
    
### a-ha moments or challenge:
#### I was able to create copy of 3D objects and tinkering with them using model types using Babylon in order to make the materials of a house. Plus, I was also able to use different properties to `const faceUV = [];` models in order to tinker with copies of a house.

### Questions I still have:
#### How to implement more basic animation and 3D objects using the challenge of making a village.

### What you're going to try next:
#### I'm going to try out [Changing the Viewer's Camera](https://doc.babylonjs.com/features/introductionToFeatures/chap2/viewer2/) and [A Walk Around The Village](https://doc.babylonjs.com/features/introductionToFeatures/chap3/walkpath/)

3.4.25
### 3.4.25
## 01/13/25
### My resources and goal:
#### My goal was to tinker with 3D objects and animation by [Creating walking character around the village](https://playground.babylonjs.com/#KBS9I5#81) which is basically making new animated character who is walking around the village and characer looks like in outside and in different sides. I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

### Before:
![Screenshot 2025-03-04 10 53 13 AM](https://github.com/user-attachments/assets/f78df15b-8abc-4046-b013-6886f05d9a49)
![Screenshot 2025-03-04 10 53 21 AM](https://github.com/user-attachments/assets/aba29b8d-4989-440c-b06c-50790fddb112)
![Screenshot 2025-03-04 10 53 49 AM](https://github.com/user-attachments/assets/dda32d5e-b609-4af4-b720-a6bbf0a012c8)

```
const track = [];
    track.push(new walk(86, 7));
    track.push(new walk(-85, 14.8));
    track.push(new walk(-93, 16.5));
    track.push(new walk(48, 25.5));
    track.push(new walk(-112, 30.5));
    track.push(new walk(-72, 33.2));
    track.push(new walk(42, 37.5));
    track.push(new walk(-98, 45.2));
    track.push(new walk(0, 47))

    // Dude
    BABYLON.SceneLoader.ImportMeshAsync("him", "/scenes/Dude/", "Dude.babylon", scene).then((result) => {
        var dude = result.meshes[0];
        dude.scaling = new BABYLON.Vector3(0.008, 0.008, 0.008);
            
        dude.position = new BABYLON.Vector3(-6, 0, 0);
        dude.rotate(BABYLON.Axis.Y, BABYLON.Tools.ToRadians(-95), BABYLON.Space.LOCAL);
        const startRotation = dude.rotationQuaternion.clone();    
            
        scene.beginAnimation(result.skeletons[0], 0, 100, true, 1.0);

        let distance = 0;
        let step = 0.015;
        let p = 0;

     const camera = new BABYLON.ArcRotateCamera("camera", -Math.PI / 1.5, Math.PI / 2.2, 15, new BABYLON.Vector3(0, 0, 0));
    camera.attachControl(canvas, true);
    const light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(1, 1, 0));

```

### Things you tried, tinkered with, your progress, etc.,:
I was confused with the purpose of certain codes including `track.push`, `const startRotation = dude.rotationQuaternion.clone();` and `scene.beginAnimation(result.skeletons[0], 0, 100, true, 1.0);` which had plenty of codes inside. All of these certain codes are materials of an speed of walking character, height, animation, position, apperance, height, rotation, and x, z which I've tinkered with so far.

### After:
![Screenshot 2025-03-04 10 50 19 AM](https://github.com/user-attachments/assets/64b0f9bc-b1ff-4d30-8d60-e259e4d33947)
![Screenshot 2025-03-04 10 51 08 AM](https://github.com/user-attachments/assets/9efc97ed-01f1-4d26-a8f5-36dc95dd2145)
![Screenshot 2025-03-04 10 51 26 AM](https://github.com/user-attachments/assets/f40f6e57-20b7-4d63-af7b-589ea13366a8)


```
const track = [];
    track.push(new walk(96, 9));
    track.push(new walk(-65, 15.8));
    track.push(new walk(-83, 17.5));
    track.push(new walk(58, 35.5));
    track.push(new walk(-122, 40.0));
    track.push(new walk(-52, 43.0));
    track.push(new walk(82, 47.0));
    track.push(new walk(-88, 55.0));
    track.push(new walk(100, 87))

    // Dude
    BABYLON.SceneLoader.ImportMeshAsync("him", "/scenes/Dude/", "Dude.babylon", scene).then((result) => {
        var dude = result.meshes[0];
        dude.scaling = new BABYLON.Vector3(0.118, 0.118, 0.118);
            
        dude.position = new BABYLON.Vector3(-9, 5, 5);
        dude.rotate(BABYLON.Axis.Y, BABYLON.Tools.ToRadians(-85), BABYLON.Space.LOCAL);
        const startRotation = dude.rotationQuaternion.clone();    
            
        scene.beginAnimation(result.skeletons[0], 5, 100, true, 1.0);

        let distance = 0;
        let step = 0.005;
        let p = 0;

     const camera = new BABYLON.ArcRotateCamera("camera", -Math.PI / 2.5, Math.PI / 4.2, 18, new BABYLON.Vector3(0, 0, 0));
    camera.attachControl(canvas, true);
    const light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(1, 1, 0));
```

### Things you learned through tinkering:

#### I learned that `track.push` ---> speed of character in every step inclduing x and y values of its speed. `const startRotation = dude.rotationQuaternion.clone();` --->  rotation of walking character,`scene.beginAnimation(result.skeletons[0], 0, 100, true, 1.0);` ---> animated characters height, appearance, and width which are showed as x and y values. 
    
### a-ha moments or challenge:
#### I was able to create character who is walking around the village of 3D objects and tinkering with them using model types using Babylon in order to make the materials of a village. Plus, I was also able to use different properties to  models in order to tinker with animation with a village

### Questions I still have:
#### How to implement more advanced animation using the challenge of making a village.

### What you're going to try next:
#### I'm going to try out [Changing the Viewer's Camera](https://doc.babylonjs.com/features/introductionToFeatures/chap2/viewer2/) 
<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->

### 3/24/25
### My resources and goal:
#### My goal was to tinker with animation by [Creating Fountain](https://playground.babylonjs.com/#TC31NV#4) which is basically making new animated fountain in a new way by tinkerimg with it and it look different in each side I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

### Before:
![Screenshot 2025-03-19 11 11 12 AM](https://github.com/user-attachments/assets/5d51ce29-5e59-4b51-b431-cd8a56207a51)
![Screenshot 2025-03-19 11 11 56 AM](https://github.com/user-attachments/assets/84fb89f2-ba27-4a3d-852e-62c573dc761a)
![Screenshot 2025-03-19 12 22 53 PM](https://github.com/user-attachments/assets/d114d8f9-94f2-4a6a-b472-ea6c68381b3f)

```
const fountainProfile = [
		new BABYLON.Vector3(0, 0, 0),
		new BABYLON.Vector3(10, 0, 0),
        new BABYLON.Vector3(10, 4, 0),
		new BABYLON.Vector3(8, 4, 0),
        new BABYLON.Vector3(8, 1, 0),
        new BABYLON.Vector3(1, 2, 0),
		new BABYLON.Vector3(1, 15, 0),
		new BABYLON.Vector3(3, 17, 0)
	];

 particleSystem.emitter = new BABYLON.Vector3(0, 10, 0); 
    particleSystem.minEmitBox = new BABYLON.Vector3(-1, 0, 0); 
    particleSystem.maxEmitBox = new BABYLON.Vector3(1, 0, 0); 

    particleSystem.color1 = new BABYLON.Color4(0.93, 0.05, 0.45);
    particleSystem.color2 = new BABYLON.Color4(0.99, 0.9, 0.08);
    particleSystem.colorDead = new BABYLON.Color4(0.82, 0.04, 0.98, 0.95);

    particleSystem.minSize = 0.1;
    particleSystem.maxSize = 0.5;

    particleSystem.minLifeTime = 2;
    particleSystem.maxLifeTime = 3.5;

    particleSystem.emitRate = 1500;
```

### Things you tried, tinkered with, your progress, etc.,:
I was confused with the purpose of certain codes including `const fountainProfile`, ` particleSystem.emitter`, `particleSystem.emitRate`, `    particleSystem.minSize`, `particleSystem.color1` , and `particleSystem.minLifeTime`  which had plenty of codes inside. All of these certain codes are materials of an speed of fountain, appearance, size, height, animation, position, rotation, and x, z, etc,. which I've tinkered with so far.

### After:
![Screenshot 2025-03-19 12 32 33 PM](https://github.com/user-attachments/assets/49efb0de-7077-47f2-bc31-53d08612586b)
![Screenshot 2025-03-19 12 32 05 PM](https://github.com/user-attachments/assets/f4d85cf2-05a2-42ae-8f3c-662ff93d0b8d)
![Screenshot 2025-03-19 12 31 48 PM](https://github.com/user-attachments/assets/3a35970b-f5cc-47bc-804a-536ca4f1357e)
![Screenshot 2025-03-19 12 33 12 PM](https://github.com/user-attachments/assets/9d7d45ee-cf3d-48bb-8454-275af080f0c2)
![Screenshot 2025-03-19 12 34 45 PM](https://github.com/user-attachments/assets/e35d0fb4-e5b4-4abf-8156-1392c0a80f44)


```
const fountainProfile = [
		new BABYLON.Vector3(1, 2, 3),
		new BABYLON.Vector3(9, 5, 2),
        new BABYLON.Vector3(9, 18, 11),
		new BABYLON.Vector3(18, 18, 12),
        new BABYLON.Vector3(15, 11, 3),
        new BABYLON.Vector3(11, 12, 11),
		new BABYLON.Vector3(11, 11, 12),
		new BABYLON.Vector3(11, 17, 12)
	];

    particleSystem.emitter = new BABYLON.Vector3(15, 7, 8);
    particleSystem.minEmitBox = new BABYLON.Vector3(-1, 10, 8);
    particleSystem.maxEmitBox = new BABYLON.Vector3(0, 1, 0);

    particleSystem.color1 = new BABYLON.Color4(0.14, 0.96, 0.04);
    particleSystem.color2 = new BABYLON.Color4(0.85, 0.2, 0.03);
    particleSystem.colorDead = new BABYLON.Color4(0.96, 0.04, 0.91, 0.96);

    particleSystem.minSize = 4;
    particleSystem.maxSize = 4;

    particleSystem.minLifeTime = 8;
    particleSystem.maxLifeTime = 8;

    particleSystem.emitRate = 2500;
```

### Things you learned through tinkering:

#### I learned that `const fountainProfile` --> shapes of the fountain not the water, ` particleSystem.emitter` --> Where the particles come from, `particleSystem.emitRate` --> Emission rate, `particleSystem.minSize` --> Size of each particle (random between max and min), `particleSystem.color1` --> Colors of all particles especially the water , and `particleSystem.minLifeTime` --> Life time of each particle (random between max and min) so they are baiscally speed, size, shape, appearance, fountain, animation, etc,.

### a-ha moments or challenge:
#### I was able to create unique fountain of my own that had different color of water and different shapes of the fountain but most importantly it is animated with 3D object fo a fountain using Babylon in order to make the new fountain. Plus, I was also able to use different properties and animation to  models in order to tinker with animated fountain.

### Questions I still have:
#### How to implement more advanced version of both 3D objects and animation using the challenge of making a fountain.

### What you're going to try next:
#### I'm going to try out [Changing the Viewer's Camera](https://doc.babylonjs.com/features/introductionToFeatures/chap2/viewer2/)

### 4/1/25
### My resources and goal:
#### My goal was to tinker with animation by [Add an animated UFO to your scene](https://playground.babylonjs.com/#KBS9I5#90) which is basically making new animated and mysterious object seen in the sky in a new way by tinkerimg with it and it look different in each side I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

### Before:
![Screenshot 2025-03-24 11 28 07 AM](https://github.com/user-attachments/assets/9aff9354-28a0-4355-bf38-02e4b9c274e8)
![Screenshot 2025-03-24 11 27 59 AM](https://github.com/user-attachments/assets/400dcef6-3616-4171-931e-2a17bbc1d81a)
![Screenshot 2025-03-24 11 27 43 AM](https://github.com/user-attachments/assets/4ab23ce6-d52b-4991-a41b-302f3bb2373a)

```
const camera = new BABYLON.ArcRotateCamera("camera", -Math.PI / 2, Math.PI / 2.5, 15, new BABYLON.Vector3(0, 0, 0));
    camera.upperBetaLimit = Math.PI / 2.2;
    camera.attachControl(canvas, true);
    const light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(1, 1, 0));

const spriteManagerUFO = new BABYLON.SpriteManager("UFOManager","https://assets.babylonjs.com/environments/ufo.png", 1, {width: 128, height: 76});
    const ufo = new BABYLON.Sprite("ufo", spriteManagerUFO);
    ufo.playAnimation(0, 16, true, 125);
    ufo.position.y = 5;
    ufo.position.z = 0;
    ufo.width = 2;
    ufo.height = 1;

    const skybox = BABYLON.MeshBuilder.CreateBox("skyBox", {size:150}, scene);
	  const skyboxMaterial = new BABYLON.StandardMaterial("skyBox", scene);
	  skyboxMaterial.backFaceCulling = false;
	  skyboxMaterial.reflectionTexture = new BABYLON.CubeTexture("textures/skybox", scene);
	  skyboxMaterial.reflectionTexture.coordinatesMode = BABYLON.Texture.SKYBOX_MODE;
	  skyboxMaterial.diffuseColor = new BABYLON.Color3(0, 0, 0);
	  skyboxMaterial.specularColor = new BABYLON.Color3(0, 0, 0);
	  skybox.material = skyboxMaterial;
```

### Things you tried, tinkered with, your progress, etc.,:
I was confused with the purpose of certain codes including `const fountainProfile`, ` particleSystem.emitter`, `particleSystem.emitRate`, `    particleSystem.minSize`, `particleSystem.color1` , and `particleSystem.minLifeTime`  which had plenty of codes inside. All of these certain codes are materials of an speed of fountain, appearance, size, height, animation, position, rotation, and x, z, etc,. which I've tinkered with so far.

### After:
![Screenshot 2025-03-24 11 41 12 AM](https://github.com/user-attachments/assets/99a97482-51d3-4811-a6e4-22e622df8f3f)
![Screenshot 2025-03-24 11 40 59 AM](https://github.com/user-attachments/assets/93637819-b53d-4029-bf7a-3f2e9d5b6dde)
![Screenshot 2025-03-24 11 40 47 AM](https://github.com/user-attachments/assets/ca313f85-ab04-46ec-afb3-e9d8528d44a6)


```
    const camera = new BABYLON.ArcRotateCamera("camera", -Math.PI / 3, Math.PI / 3.5, 20, new BABYLON.Vector3(2, 1, 2));
    camera.upperBetaLimit = Math.PI / 4.2;
    camera.attachControl(canvas, true);
    const light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(2, 1, 2));

    const spriteManagerUFO = new BABYLON.SpriteManager("UFOManager","https://assets.babylonjs.com/environments/ufo.png", 1, {width: 128, height: 76});
    const ufo = new BABYLON.Sprite("ufo", spriteManagerUFO);
    ufo.playAnimation(2, 16, true, 155);
    ufo.position.y = 8;
    ufo.position.z = 5;
    ufo.width = 4;
    ufo.height = 2;
    
    //Skybox
    const skybox = BABYLON.MeshBuilder.CreateBox("skyBox", {size:250}, scene);
	  const skyboxMaterial = new BABYLON.StandardMaterial("skyBox", scene);
	  skyboxMaterial.backFaceCulling = false;
	  skyboxMaterial.reflectionTexture = new BABYLON.CubeTexture("textures/skybox", scene);
	  skyboxMaterial.reflectionTexture.coordinatesMode = BABYLON.Texture.SKYBOX_MODE;
	  skyboxMaterial.diffuseColor = new BABYLON.Color3(0.01, 0.98, 0.06);
	  skyboxMaterial.specularColor = new BABYLON.Color3(0.97, 0.04, 0.43);
	  skybox.material = skyboxMaterial;
```

### Things you learned through tinkering:

#### I learned that `const fountainProfile` --> shapes of the fountain not the water, ` particleSystem.emitter` --> Where the particles come from, `particleSystem.emitRate` --> Emission rate, `particleSystem.minSize` --> Size of each particle (random between max and min), `particleSystem.color1` --> Colors of all particles especially the water , and `particleSystem.minLifeTime` --> Life time of each particle (random between max and min) so they are baiscally speed, size, shape, appearance, fountain, animation, etc,.

### a-ha moments or challenge:
#### I was able to create unique fountain of my own that had different color of water and different shapes of the fountain but most importantly it is animated with 3D object fo a fountain using Babylon in order to make the new fountain. Plus, I was also able to use different properties and animation to  models in order to tinker with animated fountain.

### Questions I still have:
#### How to implement more advanced version of both 3D objects and animation using the challenge of making a fountain.

### What you're going to try next:
#### I'm going to try out [Add sprite trees to your scene](https://playground.babylonjs.com/#KBS9I5#89)


