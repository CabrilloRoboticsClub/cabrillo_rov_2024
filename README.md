<h1 align="center">cabrillo_rov_2024</h1>
<h3 align="center">Cabrillo's code for the MATE ROV 2024 Competition</h3>

<br>
  <p align="center">
    Organization GitHub
    <br />
    <a href="https://github.com/CabrilloRoboticsClub"><strong>CabrilloRoboticsClub »</strong></a>
    <br />
    <br />
    <a href="https://github.com/CabrilloRoboticsClub/setup">Setup</a>
    ·
    <a href="https://github.com/CabrilloRoboticsClub/deck">Deck</a>
    ·
    <a href="https://github.com/CabrilloRoboticsClub/rov">Rov</a>
  </p>
</div>
<br>

<details>
  <summary>Table of contents</summary>
  <ol>
    <li><a href="#seahawk-ii">SeaHawk II</a>
      <ol>
        <li><a href="#ros2">ROS2</a>
        <li><a href="#software-goals">Software goals</a>
        <li><a href="#sub-teams">Sub-teams</a>
        <li><a href="#meet-the-team">Meet the team</a>
        <li><a href="#setup-">Setup</a>
        <li><a href="#deck-">Deck</a>
        <li><a href="#rov-">ROV"</a>
      </ol>
    <li><a href="#getting-started">Getting started</a></li>
    <li><a href="#run">Run</a></li>
  </ol>
</details>
<br>

---
## SeaHawk II
SeaHawk II is a project designed by a team of community college students from [Cabrillo College](https://www.cabrillo.edu/) based in Aptos, California. SeaHawk II continues Cabrillo Robotics legacy as the team prepares to compete in the 2024 [MATE](https://materovcompetition.org/world-championship) International Competition for the third year in a row. MATE challenges teams worldwide to build a Remotely Operated Vehicle (ROV) that can complete simulated real-world tasks underwater. Teams also demonstrate their robot's functionality and design rationale through marketing, documentation, a presentation, and more. Previously, Cabrillo Robotics has competed in the Pioneer division of the competition and took home first place the last two consecutive years. This year, the team takes on the challenge of developing a ROV to compete in the highest class of the competition: Explore. 

<br>

### ROS2
Much its predecessors, [SeaHawk](https://github.com/CabrilloRoboticsClub/cabrillo_rov_2023) and [Hydrozoa](https://github.com/CabrilloRoboticsClub/cabrillo_rov_2022), SeaHawk II uses The Robot Operating System (ROS). Specifically, SeaHawk uses [ROS2](https://docs.ros.org/en/foxy/index.html) for its modularity and features useful in developing software specifically for robotics. 

<br>

### Software goals
Cabrillo Robotics has great ambitions improvements and enhancements for software. Goals for the software are to make it user-friendly, easily configurable, and reliable. For ease of use, the software will be have rapid setup on factory hardware, an automatic setup, and safe shutdown. The software should allow the robot to preform photogrammetry (3d model with accurate units), hold its position in the water, and automatically correct for any external forces such as drag and disruptive thrust which cause the robot to drift off course. 

<br>

### Meet the team
| Member | Major | Bio | Sub-team | 
| :--- | :--- | :---- | :---: | 
| Orion Ellefson | Computer Science | Hello, I'm Orion Ellefson. I use They/Him pronouns, and I'm currently in my second semester at Cabrillo, majoring in Computer Science, though I might switch to something on the hardware side? Either way, I'm excited to be here. | ⭐️ 🟠 🔵 🟣 ⚪️ | 
| Isaac Eda | Electrical Engineering| I like to do engineering projects, so I'm excited to join the team. I do CAD, (f360, solidworks, KiCAD), some programming, some circuit design, 3d printing and TIG welding. |🟠 | 
| Liam Gilligan | | | 🟡 🔵 ⚪️ | 
| Massimo Ginella | | | 🔴 🟠 🟡 ⚪️ |
| Stephanie L'Heureux | Software Engineering/Mechatronics| | 🔴 🟡 | 
| Theo Paris | | My name is Theo and I have some  coding experience (self-taught for at least 4 years now). I am also taking the CS11 class as well. I used to have a 3D printer but its been a while since I've used any CAD software although I am interested in learning more. | 🟠 | 
| Alexander Rieke | | | 🟠 🟣 | 
| Michael T | Electrical Engineering | | 🔴 🟠 🟡 🟣 | 
| Kate Wolsfeld | | | 🟡 | 


<br>

### Sub-teams
**⭐️ Lead Software Engineer:** Orion Ellefson

The Cabrillo Robotics software team is divided into sub-teams:  
| Sub-team | Members | 
| :--- | :--- | 
| 🔴 **UX/input** | Michael T, Massimo Ginella, Stephanie L'Heureux | 
| 🟠 **Hardware integration** | Orion Ellefson, Theo Paris, Alexander Rieke, Isaac Eda, Michael T, Massimo Ginella|
| 🟡 **Control systems** | Liam Gilligan, Kate Wolsfeld, Michael T, Massimo Ginella, Stephanie L'Heureux | 
| 🔵 **Management** | Orion Ellefson, Liam Gilligan | 
| 🟣 **Infrastructure** | Orion Ellefson, Alexander Rieke, Michael T |
| ⚪️ **Computer vision and AI** | Orion Ellefson, Liam Gilligan, Massimo Ginella |


<br>


### [Setup »](https://github.com/CabrilloRoboticsClub/setup)
Production & development environment setup, maintenance

<br>

### [Deck »](https://github.com/CabrilloRoboticsClub/deck)
User interface for the SeaHawk ROV

<br>

### [ROV »](https://github.com/CabrilloRoboticsClub/rov)
Codebase of the SeaHawk ROV

<br>

<!-- GETTING STARTED -->

---
## Getting Started
| Operating system | Docs | 
| :---: | :--- | 
|![windows](https://github.com/CabrilloRoboticsClub/cabrillo_rov_2024/assets/96219204/17ca5854-c89f-4eac-8589-81a138e02a6d) | [ROS2_with_WSL](https://github.com/CabrilloRoboticsClub/cabrillo_rov_2024/tree/doc/doc/System%20setup) | 
|![linux svg](https://github.com/CabrilloRoboticsClub/cabrillo_rov_2024/assets/96219204/db8bf42e-1a69-4df4-aa75-152a18949f04)| TODO | 
|![apple](https://github.com/CabrilloRoboticsClub/cabrillo_rov_2024/assets/96219204/cb24582c-a7f9-4f2f-b7ec-0c75820b6719)| Rip mac users 😔| 


<br>

## Run
FIXME

<br>
