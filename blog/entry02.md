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
* I used Babylon's playground feature in order to learn more about functions of playground and shapes but previous thing I learned was my unique roof of my house.

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
