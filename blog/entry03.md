# Entry 3: FP & Tool
## Name: Dildora Norbekova
## Course: SEP11
## Period: 4
## Concept: Summary of Winter Recess
##### 2/10/25

### How I have been tinkering with Babylon during Winter Recess:

#### During the past break, I have been improving my knowledge of Babylon by learning more and more through tinkering. Specifically, I have learned functions of how to do animation using Babylon and how to create a unique animated car using Babylon. I went to [Babylon website](https://www.babylonjs.com/) and chose documents or code to tinker with like shapes, animation, positions, values, functions, car, etc., I was confused about the purpose of certain codes and funcion so I changed them to see how my result would change in order to learn what those functions do such as fram, value, positions, animation, etc,. The things I've learned includes:

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
* I used Babylon's playground feature in order to learn more about functions of playground and shapes but previous thing I learned was my unique roof of my house using [building a house]([https://doc.babylonjs.com/features/introductionToFeatures/chap2/variation](https://doc.babylonjs.com/features/introductionToFeatures/chap2/variation)/) and how to tinker with it by understanding it´s code or functions in order to change them to make it my own thing

* I made a unique roof that is completely different from the recent one by changing its scaling, rotation, position, width, height of ground, diameter, height, tessellation of my unique roof, and position of my box which made my roof to look more bigger and a little far away from our box that created my unique roof. Ground got longer through it´s new height than it´s old width.
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

* However, I was confused with what the purpose of tessellation is and why it's important. Therefore I changed my tessellation from 2 to 5 to know what it does and why it is important.

![Screenshot 2024-12-02 11 17 37 AM](https://github.com/user-attachments/assets/42d1549a-cf81-4a6a-9dbe-ee10682acf70)

* I learned that tessellation is like shape of a roof that changed how it looks like

#### Lastly, my plans for Winter recess are to complete Challenge 2 of building house by tinkering with [adding texture](https://doc.babylonjs.com/features/introductionToFeatures/chap2/material/), [materials for each house side](https://doc.babylonjs.com/features/introductionToFeatures/chap2/face_material/), and [combining meshes](https://doc.babylonjs.com/features/introductionToFeatures/chap2/combine/).


### EDP
#### Since I completed step 1 and step 2 in my Blog 1, I'm on step 3 of EDP which is brainstorming possible solutions for technology of medicine. As I mentioned in my Blog 1, problems in this career are the lack of technologies in this career. Possible solution for this problem is a simulation for technology of medicine in order to get rid of the lack of technologies in this career. However, right now I am still extending my knowledge of Babylon in order to make this simulation actually exist for real by testing code out to see what I should learn or use and what I don't need to learn at all. I plan to continue learning more and more about Babylon to learn how to make a simulation. 

### Skills
I learned 2 skills: Time Management & How to learn:

#### I learned Time Management by doing my tinkerings **ON TIME** with Babylon every week when it was assigned in order to make a simulation. I also discussed with my partner how to build a house in Babylon and how to run it. We also connected with each other to not miss deadlines for anything and to stay on task & ask for help so we used our time wisely. This skill is very important for now and future because it helps me to stay focused and to balance FP with other of my academic responsibilities. 

#### I learned Babylon on my own which is called **LOYO** (Learn On Your Own). I went to its website and found interesting codes to tinker with in order to learn so I change functions that I did not knew its purpose and how to use it, then I took screenshot and copied how result have been changed after my tinkering which taught me a lot about Babylon such as what purpose of tessellation is. Therefore, I have my learning logs with information I can use in the future for my simulation in the career of medicine. 

### Summary
#### Overall, I'm really proud to plan to make a simulation about the technology of medicine using my knowledge of Babylon and Javascript with my partner. Since, this curiosity started with my goal of becoming a PA in the future, I'll do my best to actually make this simulation exist and I won't give up at all. Therefore, I'm going to continue to keep working on this FP. 

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)

