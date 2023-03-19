<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">


  <h1 align="center">Agile Robotics for Industrial Automation Competition </h1>


</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary><h3>Table of Contents</h3></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#demo">Demo</a></li>
      </ul>
    </li>
    <li>
      <a href="#documentation">Documentation</a>
      <ul>
        <li><a href="#report">Report</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
	<li><a href="#usage">Usage</a></li>
      </ul>
    </li>
    <li><a href="#contributors">Contributors</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project



The overall project revolves around understanding and tackling various agility challenges, that a
robot might face during kitting and assembly operations. The initial step is to create a strong control system architecture to efficiently handle agility challenges in kitting and assembly operations. This will be followed by implementing functions to solve these challenges using ```ARIAC interface```, ```MoveIt```, and ```ROS```.

The robots in use are:
1. UR10 robotic arm on a linear rail that is capable of only executing kitting operation.
2. Gantry robot, with a torso and UR10 arm attached to it that can accomplish both kitting
and assembly tasks.
3. Automated Guided Vehicle (AGV) to transfer parts from kitting to assembly station.

The competition includes various ```agility challenges``` such as the inclusion of **faulty parts**, **sensor blackout**, **part flipping**, and **high priority order**. 

The final implementation of the project includes but is not limited to ```ROS/C++programming```,
```coordinate-transformation``` with *TF* library, ```trajectory planning``` using *MoveIt* interface, and strategies to tackle all agility challenges for an autonomous system for different scenarios.

Additional details regarding the tasks, scoring criteria and terminologies used can be found here. [ARIAC](https://github.com/usnistgov/ARIAC/tree/ariac2021)


<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Demo

<div align="center">


  <h4 align="center"> Kitting Task with faulty part { 3rd part was faulty - part blue} (X12 Speed)</h4>


</div>

https://user-images.githubusercontent.com/90359587/224510447-9e2fbedf-1f74-4212-8907-d94f95b08860.mp4
<div align="center">


  <h4 align="center"> Assembly Task (X8 Speed)</h4>


</div>

https://user-images.githubusercontent.com/90359587/224510520-bd0ff750-9cd9-449c-93a5-1cf4d1b1eee5.mp4
<div align="center">


  <h4 align="center"> Flipping Part (X12 Speed)</h4>


</div>

https://user-images.githubusercontent.com/90359587/224510557-a6d58515-275c-4836-b6fe-3c2a7d9ce847.mp4
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- Document and Reports -->
## Documentation

The documentation for this project can be found at this link [Documentation](https://kachappilly2021.github.io/ariac/).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Report

Detailed Report which explains the implemented architecture and approaches followed to overcome agility challenges. [Report](https://github.com/KACHAPPILLY2021/ariac/blob/main/report/Final_Report.pdf)
<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

These are the instructions to get started on the project.
To get a local copy up and running follow these simple steps.

### Prerequisites
* ROS Melodic
* Gazebo 9.15+
* ARIAC and associated dependencies. [Installation](https://github.com/usnistgov/ARIAC/blob/ariac2021/wiki/tutorials/installation.md)



### Usage

After ARIAC installation and catkin workspace creation ```ariac_ws```

1. Clone the package ```group5_rwa4``` into ```src``` of ```ariac_ws``` and build it.
   ```sh
   catkin build group5_rwa4
   ```
2. Source the workspace and then run :
   ```sh
   roslaunch group5_rwa4 ariac.launch 
   ```
3. In a seperate terminal run :
   ```sh
   rosrun group5_rwa4 My_node
   ```



<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTORS -->
## Contributors

- [Darshan Jain](https://github.com/Darshan-jain98)
- [Jeffin Johny](https://github.com/KACHAPPILLY2021)
- [Pulkit Mehta](https://github.com/pulkitmehta09)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Jeffin Johny K - [![MAIL](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jeffinjk@umd.edu)
	
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/KACHAPPILLY2021)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](http://www.linkedin.com/in/jeffin-johny-kachappilly-0a8597136)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See [MIT](https://choosealicense.com/licenses/mit/) for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com
