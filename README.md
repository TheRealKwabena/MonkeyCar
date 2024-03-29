# MONKEyCAR <img width="250" alt="Screenshot_2022-04-01_at_11 53 16-removebg-preview" src="https://user-images.githubusercontent.com/78755376/170821569-f95d97af-0c9d-4e4b-817e-6c92abe7243c.png" align="right">

<br />
<br />

## Project Desription
### :bulb: What did we make?

The goal was to create a web-based application similar to [Scratch](https://scratch.mit.edu) that teaches children how to code. However, unlike Scratch, MONKEyCAR (the name of my application) will work with the real smart-car, which will perform the actions that the child “programmed” in our app, such as "Move 10 steps forward".

<img width="415" alt="Screenshot 2022-05-25 at 19 36 09" src="https://user-images.githubusercontent.com/78755376/170335429-d73501ee-811c-49df-b4c6-d1490704640a.png" align="left">
<img width="315" alt="Screenshot 2022-05-25 at 19 39 39 copy" src="https://user-images.githubusercontent.com/78755376/170335858-2728d6b4-0395-4e51-bcf2-ef1171468f89.png">

<br />

### :yellow_heart: Our purpose

Ultimately, the main goal  was to **teach and inspire kids to code in a more fun and interactive way!** Technology is being integrated more and more into our day to day lives, with a larger number of people wanting to learn programming. However, for young children, programming might be a bit intimidating at first, and our goal is to create a user-friendly, supportive platform that will help guide them and realise that programming can be a lot of fun.

<br />



### :question: How did we plan to do it?

We had a lot of different ideas on how to implement this idea, however we soon realised that some of them were too ambitious for the context of this project. We still want to highlight some of the other ideas we had:

- Different game modes depending on difficulty
- Buttons that are written like code that you can just press (like in Scratch)
- Storing different profiles (maybe with completion points, command history, favourite programmes, ..)
- Providing some challenges (like specific actions to do with code, code with blank spaces, change code to do something different, etc)
- Leaderboards for the challenges to encourage more coding
- Adding some sounds so that the car could make cars depending on certain conditions

\
<img width="450" alt="Screenshot_2022-04-01_at_11 53 16-removebg-preview" src="https://user-images.githubusercontent.com/78755376/170821716-870581e7-bb0a-4142-9b57-3b478ebdd7b5.png" align="right">
**:sparkles: However, this is what we _finally_ envisioned MONKEyCAR to look like:**

- Code blocks that you can put together like puzzle pieces and can be executed at the same time
- Include basic movements like forward, backwards, left, right
- Teach one important programming concept like for loops or if statements
- Have some kind of canvas where the code blocks can be dragged into
- Have a play button that sends the commands to the car and a stop button that stops the execution
- Using the sensors to make sure no obstacles are hit and send a message asking the user to place the car somewhere else

<br />

### :computer: What kind of technology did we use?
We were primarily using **HTML, CSS and JavaScript** in order to develop our website and **C++** for the execution of the commands by the car.

<br />
<br />

## :airplane: Get started

If you are not working with the physical car you will need to download and setup the emulator SMCE. Below you can find specific instructions where to download it and how to start working with it. Before you do that you should clone this repository on your own device. Below you will find some information on the included files and folders and which ones are relevant for you. You will also find an explanation on what the different code blocks can do.

<br />

### Setup SMCE

Download and open SMCE [here](https://github.com/ItJustWorksTM/smce-gd/releases/tag/v1.3.4) and follow the steps below:

| <img width="500" alt="Screenshot 2022-05-25 at 19 37 42" src="https://user-images.githubusercontent.com/78755376/170339214-770db480-9e86-4880-ad81-0cfa12e07118.png"> | <img width="600" alt="Screenshot 2022-05-25 at 19 37 51" src="https://user-images.githubusercontent.com/78755376/170339279-a64f3e8d-f6fb-466f-bd8c-95d429c9efc3.png">| <img width="300" alt="Screenshot 2022-05-25 at 19 38 41" src="https://user-images.githubusercontent.com/78755376/170339286-890b2202-1036-4c31-802f-4c4ad0a3fc91.png"><img width="300" alt="Screenshot 2022-05-25 at 19 38 48" src="https://user-images.githubusercontent.com/78755376/170339289-ba46789e-d4e2-47a9-9aa4-7210d2a6b93d.png">|
|:--:| :--:| :--:| 
| *Press + to add a new arduino sketch* | *Add a new sketch* | *Select the file "smartcar.ino" from the folder "arduino"* |
| <img width="320" alt="Screenshot 2022-05-25 at 19 38 58" src="https://user-images.githubusercontent.com/78755376/170339292-300a690d-d225-4fc8-aad0-a44e2c92c4e3.png"> | <img width="300" alt="Screenshot 2022-05-25 at 19 39 06" src="https://user-images.githubusercontent.com/78755376/170339299-f9e22501-1abb-461d-8be4-b628d5ed9ba4.png">| <img width="320" alt="Screenshot 2022-05-25 at 19 39 32" src="https://user-images.githubusercontent.com/78755376/170339307-4410e53c-9e40-493f-9870-15ec00a193f5.png">|
| *Select the added sketch* | *Compile the sketch* | *Press start to run the sketch* |

<img width="578" alt="Screenshot 2022-05-25 at 19 39 39" src="https://user-images.githubusercontent.com/78755376/170339310-7d1dd91b-cd45-4f71-b531-424295432a2f.png">
This is how your screen look now. You can start setting up the webpage now.

<br />
<br />

### Using the app

<img width="470" alt="Screenshot 2022-05-29 at 15 28 42 copy" src="https://user-images.githubusercontent.com/78755376/170871460-64326620-9876-4554-8ad5-e917258cdde4.png" align="right">


- Open the file "index.html" located in the folder "gui" in a browser of your choice
- The code blocks in the selection menu on the left all represent a different action that the car can perform
- They can be dragged into the canvas on the right, where they together form a code sequence that can be executed by the car
- When the play button on top of the page is pressed the code blocks within the canvas are translated into commands that are sent either to the physical car or the emulator
- The clear button clears out all the blocks in the canvas. Before that is done it asks the user for permission.

<br />
<br />
<br />

### The code blocks

<img width="250" alt="Screenshot 2022-05-29 at 15 28 42" src="https://user-images.githubusercontent.com/78755376/170871469-76a2ba93-95ea-4f3f-a041-b60fb2ee1efb.png" align="left">


**Move x seconds forward** takes as input the number of seconds the car is supposed to drive forward.

**Move x seconds backwards** takes as input the number of seconds the car is supposed to drive backwards.

**Turn x degrees left** takes as input a degree and turns the car to the left by that number.

**Turn x degrees right** takes as input a degree and turns the car to the right by that number.

**Turn around** does not take any input but makes the car turn 180° so that it can go into the other direction.

**Spin around** does not take any input but makes the car drive spin by 360°. This does not refer to turning on the spot but rather to making a full circle

**Wait x seconds** takes as input the number of seconds the car is supposed to stand still before performing the next action

**Repeat x times** is a special block that is resembling the programming concept of for loops, instead of just executing everything sequencially. The code block has a field where all the other code blocks may be dragged into. Those code blocks are then executed x times. It is not possible to drag this code block into another "repeat x times" block.

<br />
<br />
<br />

### The buttons

<img width="592" alt="Screenshot 2022-05-29 at 15 11 05" src="https://user-images.githubusercontent.com/78755376/170870554-941d8711-5531-4cfc-b549-fc5c45545a10.png">


**Play button:**
When the play button is pressed all the elements that are inside the canvas are read and translated into commands for the car. Those are then sequentially send to the car with MQTT. When the car receives a message it executes the action specified in that message.

**Stop button:**
The stup button sends another message to the car to stop the execution of the code sequence. However, it only stops the execution of the sequence, not the execution of an action. That means that if an action like "move 10 steps forward" is not stopped until those 10 steps are finished. It simply does not execute the messaged following that action. In case you need to stop the car during one action you can make use of our obstacle avoidance and place an obstacle to the front/back of the car depending on the direction it is going in. That will stop the movement of the car immediatly. 

**Clear button:**
The clear button is used to clear all code blocks from the canvas. Before doing that however, the user is asked for confirmation.

**Trash can:**
The trash can on the right is to delete single code blocks from the canvas. The user can drag the code blocks into the trash to delete them. If a repeat block is dragged into the trash can all the blocks inside are deleted as well.

<br />
<br />



<br />
<br />

## :open_file_folder: Structure

If you want to learn a little more about how the system works, how our code is structured and how the different components work and communicate with each other this is the section for you. :point_down:

<br />

### Folder structure

The components described above can also be recognized in our folder structure. The main two folders are "gui" and "arduino" which represent the components MONKEyCar Website and SmartCar. 

**gui**

<img width="245" alt="Screenshot 2022-05-28 at 14 44 07" src="https://user-images.githubusercontent.com/78755376/170826085-27ceef3d-ed1b-4b81-a45c-dff6c5afa7b8.png" align="left">

The folder gui includes a folder called assets which consists of the pictures for buttons, our logo and the example gui. It also includes the index.html file, which includes all the html code and is supposed to be opened in a browser to use our application. Furthermore we have a folder for the JavaScript code, one for the css styles and one for the mqtt connection calles "paho.javascript-1.0.3". Note that the files in the folder "paho.javascript-1.0.3" are not written by us but downloaded from [here](https://www.eclipse.org/org/documents/edl-v10.php).

**arduino**

<img width="245" alt="Screenshot 2022-05-28 at 14 44 40" src="https://user-images.githubusercontent.com/78755376/170826526-9273e6bf-3e81-4d2f-a506-23ff06fe35d1.png" align="left">

This folder contains another folder called "smartcar" which contains the file "smartcar.ino".

<br />

### Components

The main components of our system are the GUI (and the logic for that), the MQTT broker and the arduino board running on the physical car or in the emulator. This diagram shows the basic components and how they interact with each other. In the file structure you can cleary see a separation between the arduino code and the gui. However, we do not have a folder for the mqtt broker. We are using an online broker and therefore that is running on the server "broker.emqx.io". The connection to that server from the webpage is part of the JavaScript file "script.js" as well as the folder "paho.javascript-1.0.3". The connection from the arduino side is embedded in the file "smartcar.ino".

![Untitled Diagram-2](https://user-images.githubusercontent.com/78755376/170674607-39d607f2-020f-4fd4-9105-dd95bd39ab86.png)


if you want to go into a little more detail we recommend looking at the following diagram. It further describes how our compontents interact with each other. As you can see we also added sub-components, like the sensors for the car or the relevant GUI components. Don't get confused why we have two car components. This is just supposed to showcase, that we can either work with the physical car or with the car in the emulator.

![Untitled Diagram](https://user-images.githubusercontent.com/78755376/170675070-4954cdb9-7f5c-4001-a46f-bf7f591274ad.png)


