# Entry 5: FP & Tool
## Name: Dildora Norbekova
## Course: SEP11
## Period: 4
## Concept: Babylon
##### 4/28/25

### How I have been learning Babylon and How I finished my MVP with my partner

#### During the past weeks, I successfully completed my MVP with Michaela that includes our website and our simulation using Babylon. I have been improving my knowledge of Babylon by learning more and more about how to create animations and 3D objects through tinkering. Specifically, I have learned how to do animated objects and 3D shapes using Babylon. I went to [Babylon website](https://www.babylonjs.com/) and chose [Creating Fountain](https://playground.babylonjs.com/#TC31NV#4) which is basically creating animated object of fountain that spits out unique water around the village along with advanced version of 3D objects [Add an animated UFO to your scene](https://playground.babylonjs.com/#KBS9I5#90) which is basically expanding on 3D objects to a flying object in the sky and how animated UFO looks like in outside in order to tinker with 3D objects, shapes, animation, positions, values, functions, etc., I was confused about the purpose of certain codes and funcion so I changed them to see how my result would change in order to learn what those functions do such as  3D objects, fram, value, positions, animation, etc,. The things I've learned includes:

#### My goal was to tinker with animation by [Creating Fountain](https://playground.babylonjs.com/#TC31NV#4) which is basically making new animated fountain in a new way by tinkering with it and it look different in each side I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

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
#### I was confused with the purpose of certain codes including `const fountainProfile`, ` particleSystem.emitter`, `particleSystem.emitRate`, `particleSystem.minSize`, `particleSystem.color1` , and `particleSystem.minLifeTime`  which had plenty of codes inside. All of these certain codes are materials of a fountain's speed of fountain, appearance, size, height, animation, position, rotation, and x, z, etc,. which I've tinkered with so far.

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

#### My tinkerings: I learned that `const fountainProfile` --> shapes of the fountain not the water, ` particleSystem.emitter` --> Where the particles come from, `particleSystem.emitRate` --> Emission rate, `particleSystem.minSize` --> Size of each particle (random between max and min), `particleSystem.color1` --> Colors of all particles especially the water , and `particleSystem.minLifeTime` --> Lifetime of each particle (random between max and min) so they are basically speed, size, shape, appearance, fountain, animation, etc,.

#### My challenges: I was able to create a unique fountain of my own that had different colors of water and different shapes of the fountain but most importantly it is animated with a 3D object of a fountain using Babylon in order to make the new fountain. Plus, I was also able to use different properties and animation to  models in order to tinker with animated fountains.

#### However, I still wonder how to implement more advanced versions of both 3D objects and animation using the challenge of making a fountain.

#### Additionally, I was to tinker with animation by [Add an animated UFO to your scene](https://playground.babylonjs.com/#KBS9I5#90) which is basically making new animated and mysterious object seen in the sky in a new way by tinkering with it and it look different in each side I used [Babylon](https://www.babylonjs.com/) to see various code/tools/projects that I could tinker with in order to learn more and more.

### Before:
![Screenshot 2025-03-24 11 28 07 AM](https://github.com/user-attachments/assets/9aff9354-28a0-4355-bf38-02e4b9c274e8)
![Screenshot 2025-03-24 11 27 59 AM](https://github.com/user-attachments/assets/400dcef6-3616-4171-931e-2a17bbc1d81a)
![Screenshot 2025-03-24 11 27 43 AM](https://github.com/user-attachments/assets/4ab23ce6-d52b-4991-a41b-302f3bb2373a)

```

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
#### My tinkerings: I was confused with the purpose of certain codes including `cost spriteManagerUFO`, `const skybox`, `particleSystem.emitRate`, `skyboxMaterial.diffuseColor`, `skyboxMaterial.specularColor` , and `ufo.playAnimation`  which had plenty of codes inside. All of these certain codes are materials of a fountain's speed of fountain, appearance, size, height, animation, position, rotation, and x, z, etc,. which I've tinkered with so far.

### After:
![Screenshot 2025-03-24 11 41 12 AM](https://github.com/user-attachments/assets/99a97482-51d3-4811-a6e4-22e622df8f3f)
![Screenshot 2025-03-24 11 40 59 AM](https://github.com/user-attachments/assets/93637819-b53d-4029-bf7a-3f2e9d5b6dde)
![Screenshot 2025-03-24 11 40 47 AM](https://github.com/user-attachments/assets/ca313f85-ab04-46ec-afb3-e9d8528d44a6)


```
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

#### I learned that `const spriteManagerUFO` --> height and weight of the flying object, `const skybox` --> size of the flying object, `particleSystem.emitRate` --> speed and rotation, `skyboxMaterial.diffuseColor` --> color of sky, `skyboxMaterial.specularColor` --> 2nd color of sky that are mixed together, and `ufo.playAnimation` --> speed, animation, and position.Therefore, all these certain codes are materials of an speed of UFO, appearance, size, height, animation, position, rotation, and x, z, etc,.

#### My challenge: I was able to create a unique UFO which I never saw before (LOL) of my own that had different appearances and different shapes of the flying object but most importantly it is animated with a 3D object to a UFO using Babylon in order to make the new UFO. Plus, I was also able to use different properties and animation to  models in order to tinker with animated flying objects.

#### I still wonder how to implement more advanced versions of both 3D objects and animation using the challenge of making a UFO.
#### I'm going to try out [Add sprite trees to your scene](https://playground.babylonjs.com/#KBS9I5#89)

### MVP
![Screenshot 2025-04-30 10 54 22 AM](https://github.com/user-attachments/assets/2090d8b5-e03b-4869-9af0-7a1664e478be)
![Screenshot 2025-04-30 10 54 10 AM](https://github.com/user-attachments/assets/052d193e-a220-4cf5-98d3-f0a2ea9e03a4)
![Screenshot 2025-04-30 10 53 56 AM](https://github.com/user-attachments/assets/e61b66a0-3f32-49c4-b48a-7ffba8208ff4)

* [This is the link to our MVP for code and full version](https://github.com/dildoran2195/medicalproject/blob/main/index.html)
* Below is our simulation using Babylon called Advanced Blood Tester.
![IMG_3408](https://github.com/user-attachments/assets/d2983e2f-6447-45e7-8a91-a03cd536cf00)
![IMG_3409](https://github.com/user-attachments/assets/739e1774-09de-4447-b7c8-90e4df7b3669)
![IMG_3410](https://github.com/user-attachments/assets/d0a2213f-c24d-44a2-983c-2f607c290167)

* We stayed in the library and connected with each other through messages in order to be up to date with what we have to finish and what we can improve on which gave us success so communication and connection is a key to completion. We followed the deadline and responsibilities of each other based on our plan sheet. For example, I did the CSS, Java, and simulation while my partner did HTML, Java, and Simulation because our goal was to show the general scope of medicine by considering the future and present instead of past.

### Engineering Design Process

####  Recently, I am almost done with gaining knowledge of both Javascript and Babylon in order to create a website that introduces my solution with a simulation model that positively contributes to development of medical technology so I need to merge my knowledge of those together to do so. However, Javascript and Babylon are still not enough so I am almost done with p5js in order to be on top of my website through a medical simulation model that solves lack of technologies in the medical field. Therefore, I have enough knowledge of p5js with skills and experiences which lead me to finish and plan step 5 (Create prototype). Step 5 is basically creating a functional prototype. Our prototype for step 5 is our simulation or Advanced Blood Tester using Babylon along with my tinkering, knowledge, experiences, skills, and challenges during this project with my partner which I uploaded images above for MVP. We are in the process of testing and evaluating our prototype or Advanced Blood Tester because we did not go beyond MVP yet so we are almost there.

### Skills

#### I achieved skills of Leadership and Growth Mindset.

* I learned the skill of Leadership by delegating group tasks, supporting my partner, assuming responsibility for Java, CSS, and Simulation throughout this process of completing MVP along with the simulation. Me and my partner had plan sheet or deadlines for MVP, Javascript, p5js, and Babylon to know our task, supporting each other, and taking responsibility of our own job. For example, we were kinda late in deadline to complete MVP which influenced us to try our best in order to improve my leadership skills by staying connected, doing my part, and supporting Michaela in this difficult condition. This skill builds a stronger relationship with my partner to stay connected, to support each other no matter what, and to take our responsibility in order to complete our MVP Plan which we did so we are actually starting out beyond MVP with more animation. Additionally, we were here for each other whenever we needed help during this difficult condition to get motivation along the way with inspiration. Therefore, this skill is pretty important as it helped me to be leader. 

* I learned the skill of Growth Mindset by patience, perseverance, and the courage to ask for help when needed.
For example, I was patient enough to ask for help from my partner when our link to the simulation didn't work and on slack from my friends along with Mr.Mueller about aplicativity project in order to be a leader on my task. Also, my partner and I successfully completed a website for the future which we have already started using our Growth MIndset of how we should stay patient, perseverant, and to have the courage in order to seek help when needed which will lead us to success. I was pretty patient and persevered in considering Javascript, Babylon, and p5js to successfully complete a medical simulation and planning out specific parts which we need to actually use these concepts as resources. I tried my best to have courage, patience, and perseverance at any cost during tinkering with Babylon and MVP so I could be on top of my tinkering for the best of my patience. Therefore, this skill is pretty important as it improves you to the best of your intention. 

### Summary
#### As a result, I am pretty proud of myself and my best friend (partner, Michaela) for successfully completing the best possible solution for the lack of technologies in medicine without relying on existing technologies and others. Therefore, I am proud to bring a new existing simulation for technologies of medicine and serve positive impacts both on my community and my future with my partner. Additionally, We look forward to going beyond the MVP as we have the intention to do our best.
