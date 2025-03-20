# Entry 3: FP & Tool
## Name: Dildora Norbekova
## Course: SEP11
## Period: 4
## Concept: Babylon
##### 2/10/25

### How I have been tinkering with Babylon recently:

#### During the past weeks, I have been improving my knowledge of Babylon by learning more and more about how to create animations and 3D objects through tinkering. Specifically, I have learned how to do animated characters and buildings using Babylon. I went to [Babylon website](https://www.babylonjs.com/) and chose [Creating walking character around the village](https://playground.babylonjs.com/#KBS9I5#81) which basically created animated character walking around the village along with advanced version of 3D objects [copying meshes](https://playground.babylonjs.com/#KBS9I5#78) which is basically expanding on 3D objects to a house and how a house looks like in outside in order to tinker with 3D objects, shapes, animation, positions, values, functions, etc., I was confused about the purpose of certain codes and funcion so I changed them to see how my result would change in order to learn what those functions do such as  3D objects, fram, value, positions, animation, etc,. The things I've learned includes:

#### My goal was to tinker with 3D objects [copying meshes](https://playground.babylonjs.com/#KBS9I5#78) which is basically making a copy of 3D objects to a house and how a house looks on the outside. I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

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

* I was confused with the purpose of certain codes including 'const camera`, faceUV[0]`, `const groundMat` and `places.push([1, -Math.PI / 16, -6.8, 2.5 ]);` which had plenty of codes inside. All of these certain codes are materials of an array, position, rotation, appearance, side length, width, height, house type, rotation, and x, z which I've tinkered with so far.

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

* Analysis: I learned that `const places = [];` represents each entry that is an array of house type, rotation, and x, z. I learned how to make 3D objects, shapes, how to change its functions, and how to make multiple of them at the same time using advanced Babylon. However, I mainly tinkered with its parameters, 3D shapes, height, world objects, texture, colors, array, width, material, scaling, rotation, x, y, positions, camera & light, and how to create instances from the first two that were built.

* I learned that `const faceUV = [];` is a parameter that gives multiple options to set different images on each side of the house. Also, I was confused with what functions of `faceUV = [];` represent, like which one represents which house but I was able to figure it out by tinkering so I saw their purpose, `faceUV[0]` --> rear face, `faceUV[1]`--> `front face`, `faceUV[2]`--> right side, and `faceUV[3]`--> left side.

* Therefore, I was able to create a copy of 3D objects and tinker with them using model types using Babylon in order to make the materials of a house. Plus, I was also able to use different properties to `const faceUV = [];` models in order to tinker with copies of a house.


#### Additionally, I tinkered with 3D objects and animation by [Creating walking character around the village](https://playground.babylonjs.com/#KBS9I5#81) which is basically making a new animated character who is walking around the village and looks like the outside and on different sides. I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

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

* I was confused with the purpose of certain codes including `track.push`, `const startRotation = dude.rotationQuaternion.clone();` and `scene.beginAnimation(result.skeletons[0], 0, 100, true, 1.0);` which had plenty of codes inside. All of these certain codes are materials of a walking speed, height, animation, position, appearance, height, rotation, and x, z which I've tinkered with so far.

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

* Analysis: I learned that `track.push` ---> speed of character in every step including x and y values of its speed. `const startRotation = dude.rotationQuaternion.clone();` --->  rotation of walking character,`scene.beginAnimation(result.skeletons[0], 0, 100, true, 1.0);` ---> animated characters height, appearance, and width which are showed as x and y values. 

*Therefore, I was able to create a character who is walking around the village of 3D objects and tinkering with them using model types using Babylon in order to make the materials of a village. Plus, I was also able to use different properties to  models in order to tinker with animation with a village


### Engineering Design Process

Since I completed steps 1 through 3, now I am planning the most promising solution in order to solve the problem of lacking technologies in medicine that I figured out in step 1 (brainstorming) which is basically step four in this case. Currently, I am almost done with gaining knowledge of both Javascript and Babylon in order to create a website that introudces my solution with a simulation model that positively contributes to development of medical technology so I need to merge my knowledge of those together to do so. However, Javascript and Babylon are still not enough so I just have to finish off p5js in order to be on top of my website through a medical simulation model that solves lack of technologies in the medical field. Therefore, I have to sucessfully complete p5js with skills and experiences which leads me to finish and plan step 5 which is eventually creating a functional prototype adn this is my plan for Blog 5 along with new tinkering on my tool list.

### Skills

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
