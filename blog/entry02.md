# Entry 2
##### 12/15/24

### How I have been tinkering with Babylon and my plans for Winter Recess

#### During the past weeks, I have been improving my knowledge of Babylon by learning more and more through tinkering. Specifically, I have learned functions of shapes and playground like parameters, positions, etc,. and how to create unique house using Babylon. I went to [Babylon website](https://www.babylonjs.com/) and chose document or code to tinker with like shapes, playground, and house. I was confused about purpose of certain codes and funcion so I changed them to see how my result would change in order to learn what those functions does such as parameters, positions, etc,. The things I've learned includes:

* I learned light density is the amount of color in a playground that has only a sphere. I didn't like the shape of the sphere because it was so common so I used this code by doing code below:
```
// Our built-in 'goldenberg' shape. var sphere = BABYLON.MeshBuilder.CreateGoldberg("Goldenberg", {diameter: 2, segments: 32}, scene); // Move the goldenberg upward 1/2 its height sphere.position.y = 1;
```
![Screenshot 2024-12-16 9 16 35 AM](https://github.com/user-attachments/assets/ed7c4bf9-81df-4b48-ad8b-21c2edc3c93d)

* I learned that light.density changed how shape is shown, either dark or light and I increased light.density. Diameter is width and segment is like size of the shape or height. sphere.position is where the shape is located by creating code below:
```
// Default intensity is 1. Let's dim the light a small amount
    light.intensity = 0.5;

// Our built-in 'sphere' shape.
    var sphere = BABYLON.MeshBui!
lder.CreateSphere("sphere", {diameter: 5, segments: 50}, scene);

// Move the sphere upward 1/2 its height
    sphere.position.y = 2;
```
* I used Babylon's playground feature in order to learn more about functions of playground and shapes but previous thing I learned was my unique roof of my house using [building a house](https://doc.babylonjs.com/features/introductionToFeatures/chap2/variation/) and how to tinker with it by understanding it´s code or functions in order to change them to make it my own thing

* Also, I made a unique roof that is completely different from the recent one by changing its scalling, rotation, position, width, height of ground, diamater, heaight, tesselaion of my unique roof, and position of my box which made my roof to look more bigger and a little far away from our box that created my unique roof. Ground got more longer through it´s new height than it´s old width.
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

* However, I was confused with what purpose of tesselation is and why it´s important. Therefore I changed my tesselation from 2 to 5 to know what it does and why it is important.

![Screenshot 2024-12-02 11 17 37 AM](https://github.com/user-attachments/assets/42d1549a-cf81-4a6a-9dbe-ee10682acf70)

* I learned that tesselation is like shape of a roof that changed how it looks like

#### Lastly, my plans for Winter recess are to complete Challenge 2 of building house by tinkering with [adding texture](https://doc.babylonjs.com/features/introductionToFeatures/chap2/material/), [materials for each house side](https://doc.babylonjs.com/features/introductionToFeatures/chap2/face_material/), and [combining meshes](https://doc.babylonjs.com/features/introductionToFeatures/chap2/combine/).














[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
