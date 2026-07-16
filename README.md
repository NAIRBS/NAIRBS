<!-- Technically, I should download the files and host them myself to prevent components from breaking due to cascading third-party dependencies that I cannot control. Practically, I'm kinda too lazy to do that, and I believe in Giphy as it serves media across Meta's services as an official provider. --> 
Hi <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="40" /> My name is Brian Soh.
==================================================================================================================================

Computer Engineer
-----------------

I've been coding in academic projects for a few years, but I haven't built anything real...until now? (Will update later)

* 🖥️  Read my Blog at [Blog](http://nairbs.github.io/)
* ✉️  You can contact me at [sohhanyu@gmail.com](mailto:sohhanyu@gmail.com)
* 🚀  I'm currently working on [my blog](http://nairbs.github.io/)
* 🧠  I'm currently learning React, Node.JS, Javascript/Typescript, PostgreSQL
* 💬  Technically, I have some experience creating applications with C, C++, C#, .NET, Java, JavaScript, Python, PowerShell/Batch/Bash Scripting, HTML/CSS, but it's been years since I've touched them.

I am working on learning (or have learnt) the following stacks:
<p align="left">
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/javascript-colored.svg" alt="JavaScript" title="JavaScript" width="36" height="36" /></a><a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/typescript-colored.svg" alt="TypeScript" title="TypeScript" width="36" height="36" /></a><a href="https://www.python.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/python-colored.svg" alt="Python" title="Python" width="36" height="36" /></a><a href="https://www.gnu.org/software/bash/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/gnubash-colored.svg" alt="GNU Bash" title="GNU Bash" width="36" height="36" /></a><a href="https://code.visualstudio.com/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/visualstudiocode-colored.svg" alt="VS Code" title="VS Code" width="36" height="36" /></a><a href="https://developer.mozilla.org/en-US/docs/Glossary/HTML5" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/html5-colored.svg" alt="HTML5" title="HTML5" width="36" height="36" /></a><a href="https://reactjs.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/react-colored.svg" alt="React" title="React" width="36" height="36" /></a><a href="https://nodejs.org/en/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/nodejs-colored.svg" alt="NodeJS" title="NodeJS" width="36" height="36" /></a><a href="https://ubuntu.com/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/ubuntu-colored.svg" alt="Ubuntu" title="Ubuntu" width="36" height="36" /></a>
</p>

### Socials

<p align="left"><a href="https://www.github.com/NAIRBS" target="_blank" rel="noreferrer"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/github-dark.svg" /><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/github.svg" /><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/github.svg" width="32" height="32" alt="GitHub" title="GitHub" /></picture></a><a href="https://www.linkedin.com/in/brian-soh-9bb35724a/" target="_blank" rel="noreferrer"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin-dark.svg" /><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin.svg" /><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin.svg" width="32" height="32" alt="LinkedIn" title="LinkedIn" /></picture></a></p>

# Some of my Past Projects

## Web-Based AR with Real-Time SLAM (Academic Project) ~2025
Developed an augmented reality system featuring real-time SLAM running directly in the browser via WebAssembly. 
* Built using **C++, JavaScript (ThreeJS), WebAssembly, and HTML/CSS** (and various other things).
* Runs on Mobile, Mobile but with Google Cardboard-like distortion (Fragment Shaders), Desktop/Laptop, WSL and Nvidia Jetson NX (embedded AI supercomputer). All had serviceable performance for AR.
* Includes extensive data and event logging (real-time applications are really hard to optimise without logs) and a side panel 3D view to check if SLAM is working appropriately (display works on all platforms mentioned above).
* Definitely not production-grade software, SLAM fails inevitably given device constraints and after extended use, the backend and loop closure were disabled to maximise performance on CPU-bound hardware; the system acted more as a short-term Visual Odometry system, which was sufficient for AR Ruler/Video Player use cases.
* Github Actions (CI/CD Configs), ROS2 Nodes, bash scripting, ThreeJS, JavaScript state management and more were also used. Tried to do true wireless streaming of frames instead of wired input, but latency was just too high with free webstreaming options...
* Found to be more accurate than iOS and Android AR Ruler apps today across different lighting and environment scenarios, the D435i RGB-D stereo camera was supplied by the school, so the project used that as the input device, but technically any stereo camera with a high enough resolution (maybe around $100) should also work if the user modifies the right files to account for changes in resolution.
* **Repository:** [AlvaAR-Ubuntu-20.04](https://github.com/NAIRBS/AlvaAR-Ubuntu-20.04)
* **OS Specific Written Documentation and Setup:** [ORBSLAM3-Ubuntu-20.04](https://github.com/NAIRBS/ORBSLAM3-Ubuntu-20.04)

Try the below demo here: [Video Stream AR Ruler Visualizer](https://nairbs.github.io/AlvaAR-Ubuntu-20.04/examples/public/rgbd_video_AR_Ruler_visualizer.html)
![AR Ruler](https://github.com/user-attachments/assets/fa7505c0-54e9-4764-b0fb-5f062d9b4910)

[Video Stream Video Player](https://nairbs.github.io/AlvaAR-Ubuntu-20.04/examples/public/rgbd_video_player.html)

[Wearable Mobile AR Barrel Distorted Video Player, click anywhere after start](https://nairbs.github.io/AlvaAR-Ubuntu-20.04/examples/public/video_rgbd_video_player.html)

![chrome_rXAHypeoSY](https://github.com/user-attachments/assets/da3eefbf-2a30-411a-ba67-e10a1ac34f76)

[Wearable Mobile AR Barrel Distorted AR Ruler](https://nairbs.github.io/AlvaAR-Ubuntu-20.04/examples/public/rgbd_video_AR_Ruler_Mobile_visualizer.html)
<img width="2393" height="1114" alt="image" src="https://github.com/user-attachments/assets/f6a7468a-a54b-4f10-8631-e932797a64cd" />

## [Prototype] Course Planner for University courses (Academic Project) ~2024
Developed the frontend for a complex course planner that accommodates incomplete, malformed, and fragmented course data, multiple user configurations and parses data from the backend's recommended planning based on user constraints. 
- Allowed users to log in and out; all data was stored and managed through a local database and web server.
- Much thought was put into making the table easy to read at a glance while allowing users to see the full details of each course in the schedule.
- Allowed users to browse through different timetable configurations suggested by the system.
- Frontend built with **HTML/CSS/Javascript**. (Inline JS is considered bad practice but was used for more rapid prototyping)
* **Repository:** [SimplyStars-Course-Planner-Prototype](https://github.com/NAIRBS/SimplyStars-Course-Planner-Prototype)
<img src="https://github.com/NAIRBS/SimplyStars-Course-Planner-Prototype/assets/86892301/921a61c7-e607-4fa5-83e4-d880322af366" alt="Image" width="1200"/>

## [Prototype] Carousell Clone (Academic Project) ~2017
* Users can create accounts to buy and sell items. (With Firebase APIs).
* Users could change their account information and profile pictures.
* Image and account hosting with Firebase.
* Users could change their item listing details or delete their item listing entirely. Was a live app at the time.
* Used **Firebase backend and Java to create an Android application**.
* **Repository:** [ReMart-Ecommerce-Platform-Prototype](https://github.com/NAIRBS/ReMart-Ecommerce-Platform-Prototype)
<center>
<img src="https://github.com/NAIRBS/ReMart-Ecommerce-Platform-Prototype/assets/86892301/7519aeb9-edfc-4359-ae3e-678187bed6c3" alt="Image" width="200"/>
<img src="https://github.com/NAIRBS/ReMart-Ecommerce-Platform-Prototype/assets/86892301/fe405304-346a-4884-9021-4e1d060a90fa" alt="Image" width="200"/>
<img src="https://github.com/NAIRBS/ReMart-Ecommerce-Platform-Prototype/assets/86892301/61df0935-55f2-4648-857e-88b962ee9503" alt="Image" width="200"/>
</center>

<!-- Commented out since deployment is paused by owner? 
### Badges
<b>My GitHub Stats</b>

<a href="http://www.github.com/NAIRBS"><img src="https://github-readme-stats.vercel.app/api?username=NAIRBS&show_icons=true&hide=&count_private=true&title_color=0891b2&text_color=ffffff&icon_color=0891b2&bg_color=1c1917&hide_border=true&show_icons=true" alt="NAIRBS's GitHub stats" /></a>

<a href="https://github.com/NAIRBS" align="left"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=NAIRBS&langs_count=10&title_color=0891b2&text_color=ffffff&icon_color=0891b2&bg_color=1c1917&hide_border=true&locale=en&custom_title=Top%20%Languages" alt="Top Languages" /></a>
-->
