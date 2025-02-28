# Entry 3: FP & Tool
## Name: Dildora Norbekova
## Course: SEP11
## Period: 4
## Concept: Summary of Winter Recess
##### 2/10/25

### How I have been tinkering with Babylon during Winter Recess:

#### During the past break, I have been improving my knowledge of Babylon by learning more and more about how to create 3D objects through tinkering. Specifically, I have learned functions of how to do animated buildings using Babylon and how to create a unique 3D objects by making copy of it. I went to [Babylon website](https://www.babylonjs.com/) and chose [copying meshes](https://playground.babylonjs.com/#KBS9I5#78) which basically created 3D objects and copying houses to make multiple of them in order to tinker with 3D objects, shapes, animation, positions, values, functions, etc., I was confused about the purpose of certain codes and funcion so I changed them to see how my result would change in order to learn what those functions do such as fram, 3D objects, value, positions, animation, etc,. The things I've learned includes:

* I learned `places push` is an array that represents house type, rotation, as x, z in order from 1st varibale to last variable. I tinkered with it to see it´s changes so I will learn purpose of those functions which were all an array that represents house type, rotation, as x, z. Below is my tinkerings:
```
    places.push([2, -Math.PI / 15, -6.5, 2.9 ]);
    places.push([1, -Math.PI / 14, -4.8, 4 ]);
    places.push([3, -Math.PI / 11, -1.3, 6 ]);
    places.push([1, -Math.PI / 5, 1.8, 9 ]);
    places.push([2, 15 * Math.PI / 15, -6.3, -1.2 ]);
    places.push([2, 15 * Math.PI / 14, -4.5, -6 ]);
    places.push([1, 15 * Math.PI / 19, -2.5, -0.3 ]);
    places.push([2, 5 * Math.PI / 8, 0, -3 ]);
    places.push([2, Math.PI + Math.PI / 2.8, 0.1, -2 ]);
    places.push([1, Math.PI + Math.PI / 2.9, 0.55, -2 ]);
    places.push([2, Math.PI + Math.PI / 2.65, 0.95, -5 ]);
    places.push([1, Math.PI / 5.5, 9.35, -9 ]);
    places.push([2, Math.PI / 2.95, 8.5, -9 ]);
    places.push([1, Math.PI / 4.9, 9.75, -9 ]);
    places.push([2, Math.PI / 3.9, 7.45, -9 ]);
    places.push([1, -Math.PI / 7, 5.55, 9 ]);
    places.push([2, -Math.PI / 7, 3, 9 ]);
```

* Images below are results of my tinkerings:

## Before
![Screenshot 2025-02-24 11 05 41 AM](https://github.com/user-attachments/assets/069d1921-84b2-4957-8754-f52a1cdb15fa)

## After
![Screenshot 2025-02-24 11 17 41 AM](https://github.com/user-attachments/assets/ecd1cc1d-6dc4-4814-ba69-a0182e0925d4)

* I learned that  const `faceUV = [];` is parameter that gives multiple options to set different images on each side of house. Also, I was consused with what functions of  `faceUV = [];` represent, like which one represents whhich house but I was able to figure it out by tinkering so I saw their purpose, `faceUV[0]` --> rear face, `faceUV[1]`--> front face, `faceUV[2]`--> right side, and `faceUV[3]`--> left side. Below is my tinkerings:
```
   const faceUV = [];
    if (width == 30) {
        faceUV[0] = new BABYLON.Vector4(1.6, 1.0, 1.0, 1.0); 
        faceUV[1] = new BABYLON.Vector4(1.0, 1.0, 1.4, 1.0);
        faceUV[2] = new BABYLON.Vector4(1.4, 1, 1.6, 1.0);
        faceUV[3] = new BABYLON.Vector4(1.4, 1, 1.6, 1.0); 
```
* I used Babylon's 3D object challenge steps in order to learn more about 3D objects, functions of playground and shapes but previous thing I learned was making a unique roof that is completely different from the recent one by changing its scaling, rotation, position, width, height of ground, diameter, height, tessellation of my unique roof, and position of my box using [building a house]([https://doc.babylonjs.com/features/introductionToFeatures/chap2/variation](https://doc.babylonjs.com/features/introductionToFeatures/chap2/variation)/) Also, how to tinker with it by understanding it´s code or functions in order to learn them to make it my own process.

* I learned how to make 3D objects, shapes, how to change it´s functions, and how to make multiple of them at the same time using advanced Babylon. However, I mainly tinkered with its parametrs, 3D shapes, height, world objects, texture, colors, array, width, material, scalling, rotation, x, y, positions, camera & light, and how to create instances from the first two that were built. Below are my tinkerings from top to bottom of my result:
```JS
const box = BABYLON.MeshBuilder.CreateBox("box", {});
    faceUV[0] = new BABYLON.Vector4(1.6, 1.0, 1.0, 1.0); 
    const camera = new BABYLON.ArcRotateCamera("camera", -Math.PI / 4, Math.PI / 3.5, 11, new BABYLON.Vector3(0, 0, 0));
    const light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(2, 2, 1));
    groundMat.diffuseColor = new BABYLON.Color3(0, 0.93, 1);
    const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:25, height:26});
    const box = BABYLON.MeshBuilder.CreateBox("box", {width: width, faceUV: faceUV, wrap: true});
    box.position.y = 0.5;
    const roof = BABYLON.MeshBuilder.CreateCylinder("roof", {diameter: 1.3, height: 1.2, tessellation: 3});
    roof.material = roofMat;
    roof.scaling.x = 1.75;
    roof.scaling.y = width;
    roof.rotation.z = Math.PI / 2;
    roof.position.y = 2.22;
```
![Screenshot 2025-02-24 3 41 36 PM](https://github.com/user-attachments/assets/eec3114d-55fb-4070-bfa9-370d85ab32f7)

* However, I was confused with what the purpose of `const places = [];` is and why it's important. Therefore I changed my `const places = [];` from it´s original variables to new variables to know what it does and why it is important.

![Screenshot 2025-02-24 3 51 32 PM](https://github.com/user-attachments/assets/e1d60b94-efcf-4e99-b028-6da727b9c4d5)


* I learned that `const places = [];` represents each entry that is an array of house type, rotation, and x, z

#### Lastly, my plans for continuing to process my tinkerings of how to create 3D objects using Babylon for our medical simulation is to complete [Changing the Viewer's Camera](https://doc.babylonjs.com/features/introductionToFeatures/chap2/viewer2/) and [A Walk Around The Village](https://doc.babylonjs.com/features/introductionToFeatures/chap3/walkpath/)


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

