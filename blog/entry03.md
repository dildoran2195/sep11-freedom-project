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

#### Since I completed step 2 in my Blog 1, I'm on step 4 of EDP which is planning the most promising solutions for technology of medicine. As I mentioned in my Blog 2, best solution for the lack of technologies is a simulation for technology of medicine in order to get rid of the lack of technologies in career of healthcare and medicine by extending knowledge of Babylon. Our planning for the most promising solutions is still a simulation for lack of technology in medicine because we brainstormed possible solutions since step 1 but we still have to plan the best efficient solution. However, we are still in process of extending information which we defined it during brainstorming the possible solutions because these plans would help a lot to build a final solution in order to fix lack of technologies in medicine using Babylon. Our plan is to create a prototype using Babylon which is step 5 after we test our various codes from Babylon. 

### Skills

* I achieved skills of Paying Attention to Small Details and Consideration

#### I learned skill of paying attention to small details. I wanted to consider every small details when learning more about 3D objects or Babylon so I decided to break it down into small pieces by tinkering every part and having enough time for each details. For example, I started to tinker with parametrs on first day then moved onto 3D shapes, height, world objects, texture, colors, array, width, material, scalling, rotation, x, y, positions, camera & light, and how to create instances from the first two that were built. Therefore, every small details built the final result successfully. Also, I paid attention to small details by breaking down both my academics with Babylon so I would have enough time to consider every small details since final result of my tinkerings above would not exist without every small details which came together successfully. Therefore, I will definitely use paying attention to small details as my resource in order to build a simulation in the career of medicine. 

#### I learned skill of Consideration by considering every small details and itś impacts which built on my skill of paying attention to every small details. I considered impacts of my tinkerings by taking notes which were learning 3D objects since it is very important for our simulation of technology in medicine so I believed that considering leads to success. For example, I considered every function in 3D objects which taught me that `const places = [];` represents each entry that is an array of house type, rotation, and x, z. Also, these consdierations would be my resources when building a simulation in the career of medicine. Plus, Babylon resources that I used to tinker were created by other people which I considered and put sources to give them credit for their work. However, consideration could sometimes be too much if you are also considering too many details so it is always bets to break it up so you want get overwhelmed so you could use those considertaion any time in the future.  

### Summary
#### Finally, I am pretty excited to extend best possible solution for lack of technologies in medicine without relying on existing technologies and others. However, I am excited to make a simulation for technologies of medicine and serving positive impacts both on my community and my future. Speaking of future, I changed future career of mine to Nurse Practicioner so I would do my best to  continue my curoisty of a medical simulaation which bulds up my future career wuth my partner and using Babylon especially 3D objects. Therefore, I'm going to extend my efforts on this FP by breaking it down into pieces.  


[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)

