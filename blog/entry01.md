# Entry 1: FP & Tool
## Name: Dildora Norbekova
## Course: SEP11
## Period: 4
## Concept: FP & Tools
##### 11/26/2024

## Why The Medicine Technology Process?

#### The topic that I have chosen for the year-long project is **The Medicine Technology Process** and my tool is **Babylon** in order to make a simulation. I chose this topic because I love to study different kinds of the technology of med and the process of making it. I am obsessed with the different styles of technologies for medicine and want to know more about it, especially all kinds of new style ones. There are plenty of technology of medicine including robotics, AI, Health administrations, Health wearables, and bioprinting which all are medical technology that can be defined as the technologies that diagnose, treat and/or improve a person's health and wellbeing. These technologies are like magical because they are able to save ones live in modern world. Also, I´m working with Michaela who is also passionate about technology of medicine and I´m very happy to work with her because we have same goal for this FP which is to do our best. Lastly, my tool for my backup project idea is Vue and my idea is probabyly Med instructive gallery. 

#### The two main links that I used to explore was [Medical Technology Facts](https://www.lifechanginginnovation.org/medical-technology-facts.html) and [Benefits Of Medical Technology: What's the Impact?](https://blog.cloudticity.com/benefits-of-medical-technology). The first link helps me know what the field medical technology is. Also, the second link tells me avantages of medical technology. Some other links that I had explored were [15 Tech Tools And Processes That Are Transforming The Healthcare Industry](https://www.forbes.com/councils/forbestechcouncil/2022/10/31/15-tech-tools-and-processes-that-are-transforming-the-healthcare-industry/) and [25 Different Types of Medical Assistant Equipment](https://medassisting.org/medical-assistant-equipment-a-comprehensive-guide/). These two were links that helped me understand the intro of medicine proess and what were devices/technology that were helpful in medical field. 

## Tinkerings with Babylon

#### I tinkered with Babylon a lot and learned so many things about it inclduing what Babylon is, parameters, positioning, etc., More at [My Tinkerings with Babylon](https://github.com/dildoran2195/sep11-freedom-project/edit/main/tool/learning-log.md).

#### Code below helped me to learn that `light.density` changed how shape is showen, either dark or light and I increased `light.density`. `Diameter` is width and `segmnet` is like size of the shape or height. `sphere.position` is where the shape is located and these were things that I was confused with. 

```
 // Default intensity is 1. Let's dim the light a small amount
    light.intensity = 0.5;

    // Our built-in 'sphere' shape.
    var sphere = BABYLON.MeshBui!
lder.CreateSphere("sphere", {diameter: 5, segments: 50}, scene);

    // Move the sphere upward 1/2 its height
    sphere.position.y = 2;
```
#### my a-ha moment in tinkering was when I did not know what tesselation is and why it´s important. Therefore I changed my tesselation from 2 to 5 to know what it does and why it is important using code and screenshot below. 
```JS
const box = BABYLON.MeshBuilder.CreateBox("box", {});
    box.position.y = 0.8;
    const roof = BABYLON.MeshBuilder.CreateCylinder("roof", {diameter: 2.2, height: 1.8, tessellation: 3});
    roof.scaling.x = 1.00;
    roof.rotation.z = Math.PI / 2;
    roof.position.y = 2.11;
    const ground = BABYLON.MeshBuilder.CreateGround("ground", {width:5, height:15});
```
![Screenshot 2024-12-02 11 17 37 AM](https://github.com/user-attachments/assets/42d1549a-cf81-4a6a-9dbe-ee10682acf70)
#### This code and screenshot taught me that tesselation is like shape of a roof that changed how it looks like

## EDP

#### The EDP stands for Engineering Design Process and my steps of the EDP are the (Step 1) defining the problem in medicine which was lacking technology in the field of medicine and the (Step 2) was researching the problem. At first, I found what I´m passionate about by defining it which was simulation for medicine technology and I found out the problem in technology of medicine which was lack of technologies in this career. Also, I did more research in the field of medicine in order to make a simulation out of it and technology that is used in medicine. For example. augmented reality, mixed reality, immersive reality and high-quality haptics are all technologies used for a simulation in medicine in order to identify the problem in a persons health. My next step would be brainstorming the solution. 

## Skills
#### I gained 3 skills: Communication, How to Google, and How to read

#### First skill that I gained was communication. I communicated with my partner by asking and helping each other to do our writeups and tinkerings. Also, we worked together in order to identify what we are passionate about. Then, choosing tool and defining the problem in the field of medicine in order to create a simulation together. I also improved my communication skill because before I was nervous to ask a question or to talk with my peers. After I imporved this skill, I did felt comfortable working with my partner in order to talk about our goals and problems that we are experiencing through FP. 

#### Another skill that I learned during this experience is **How to Google**. Since, Googling was important and allowed in order to find out more about different technologies for our different field of careers. When I looked up "med tech" I was not able to find enough information because I was not good at Googling by typing specific things that I need to know. But after I gained this skill, I learned to be more specific and add more details to my question to ask from Google. Therefore, I typed "technologies in the field of medicine process or a simulation" which gave me enough information to learn and consider through out this FP. This skill helped me to believe that I´m enough interested in this field and to do more research about future technology of medicine.  

#### Last skill that I gained was **How to Read**. Achieving skill of Googling was not enough because I supposed to have ability to understand and consider inofrmation that Google gave me based on my specific question. Before I gained this skill, I just use to try to understand terms that I did not know because I just thought it didn´t matter. However after I gained this skill, I learned that everything matters when reading an article or visiting website to learn more about medicine because all teaches something that is part of my researching. For example, when Google gave me a bunch of technologies that I did not know what it does, I read more closely about decsriptions of those technologie which were diagnosing health problem of a person by using that technology as tool to do it.

## Summary

Overall, I'm really excited to make a website about the technology of architecture. It all started with the inspiration of a restaurant in Fort Hamilton, and maybe I'll have a future career in architecture!

[Next](entry02.md)

[Home](../README.md)
