## Flutter Programmaing Assistant System with Docker

1. ⚙️ [About the System](#1-about-the-system) 
2. 🔨 [Prerequisites](#2-prerequisites) 
3. 🖥 [Follow the procedure according to OS](#3-procedure-according-to-OS) 
	- [Windows](#windows)
	- [Linux (Ubuntu)](#linux-Ubuntu)
	- [MacOS](#macos)
		- [Intel Processor](#macos-intel-processor)
		- [M1/2/3 Chip Processor](#macos-m-chip-processor) 
4. 📜 [About Exercises](#4-about-exercises) 
	- [Exercise-1](#exercise-1)
	- [Exercise-2](#exercise-2)
	- [Exercise-3](#exercise-3)
 	- [Exercise-4](#exercise-4)
  	- [Exercise-5](#exercise-5)
5. 📑 [Answer File](#5-answer-file) 
6. 📝 [Answer File Submission & System Usage Feedback ](#6-answer-file-submission-links) 

<hr style="border-top: 2px solid #333;">

## 1. About the System 
<p align="justify"> 
Flutter Programmaing Learning Assistant System includes frontend, backend and webserver.
You can see the details of the system user web pages step by step in the link below.
<a href="https://github.com/lynnhtetaung/flutter-web/wiki/FPLAS-System" style="font-size: 0.1px; color: #FF0000;">Details </a> (Right-click to open in new tab)

</p>

<p align="center">
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>
<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 2. Prerequisites 

	|                                                        Tool                                                        | Install | URL                                                                                                     |
	| :---------------------------------------------------------------------------------------------------------------------------: | :-------------: | ------------------------------------------------------------------------------------------------------- |
	| <img height="50" src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/git.png"> |      GitHub       | <ul><li>https://git-scm.com/downloads/</li></ul> |
	| <img height="50" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/74b958e4-8211-481c-8454-8aa7a719ce8b"> |      Docker       | <ul><li>https://www.docker.com/products/docker-desktop</li></ul>|

- <strong>If necessary,</strong> please download & reference the following user manual [fplas_docker.pdf](https://github.com/lynnhtetaung/fplas-2024/blob/blog/fplas_docker.pdf) for Docker Desktop.
	
<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 3. Procedure according to OS
- Depending on the Operating System, the way is different. Therefore, please follow the procedure according to the conrrespondence OS.
##

### Windows

> **Get** 3 docker images, which has FPLAS's frontend, backend and nginx environments.
```
docker pull 24091997/fplas-backend-2024:v1
docker pull 24091997/fplas-nginx-2024:v1
docker pull 24091997/fplas-frontend-2024:v1
```

> **Go** the Desktop directory****

```
cd Desktop
```

> **Clone** the project from Github, which has
- docker-compose.yml to execute pulled 3 docker images.
```
git clone https://github.com/lynnhtetaung/fplas-2024.git
```

> **Modify** the line 8 to be the same with your PC Desktop directory
- from **- /home/lynnhtetaung/Desktop/results:/app/addon/output** to
```
eg. /c/your_pc_username/Desktop/results:/app/addon/output or C:/Users/username/Desktop/results:/app/addon/output
```

> **Run** the command to start the Docker containers ****

```
docker compose up
```


> **Open** Chrome browser and navigate to **http://localhost:4000/**

<p align="center">
 <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>


<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">

### Linux (Ubuntu)
> **Get** 3 docker images, which has FPLAS's frontend, backend and nginx environments.
```
docker pull 24091997/fplas-backend-2024:v1
docker pull 24091997/fplas-nginx-2024:v1
docker pull 24091997/fplas-frontend-2024:v1
```

> **Go** the Desktop directory****

```
cd Desktop
```

> **Clone** the project from Github, which has
- docker-compose.yml to execute pulled 3 docker images.
```
git clone https://github.com/lynnhtetaung/fplas-2024.git
```

> **Modify** the line 8 to be the same with your PC Desktop directory
- from **- /home/lynnhtetaung/Desktop/results:/app/addon/output** to
```
eg. - /home/your_pc_username/Desktop/results:/app/addon/output
```

> **Run** the command to start the Docker containers ****

```
docker compose up
```


> **Open** Chrome browser and navigate to **http://localhost:4000/**

<p align="center">
 <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>


<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">

### MacOS (Intel Processor, M Chip Processor)
> Apple's transition from Intel processors to its custom-designed chips (M1/2/3), starting with the M1 and subsequent iterations. Before their transition, Apple Mac computers used Intel processors. It is provided for both Intel and M chip processors.
##
> **Get** 3 docker images, which has FPLAS's frontend, backend and nginx environments.
```
docker pull 24091997/fplas-backend-2024-ios:v1
docker pull 24091997/fplas-nginx-2024-ios:v1
docker pull 24091997/fplas-frontend-2024-ios:v1
```

> **Go** the Desktop directory****

```
cd Desktop
```

> **Clone** the project from Github, which has
- docker-compose.yml to execute pulled three docker images.
```
git clone https://github.com/lynnhtetaung/fplas-2024.git
```

> **Modify** the line 8 to be the same with your PC Desktop directory
- from **- /home/lynnhtetaung/Desktop/results:/app/addon/output** to
```
eg. /Users/username/Desktop/results:/app/addon/output
```


> **Run** the command to start the Docker containers ****

```
docker compose up
```

> **Open** Chrome browser and navigate to **http://localhost:4000/**

<p align="center">
 <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>


<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">


## 4. About Exercises
> Student can see 5 sample flutter exercises in the FPLAS's web page via browser. Students need to modify these exercises according to the modification guidance. 
### Exercise-1

> **Read** the modification gudiance and **Modify** the given source codes as same as **expected result**.
      
![e1](https://github.com/soethandaraung395/YASASHI-NPLAS/blob/docker-deploy/public/images/exercise1.png)

> [!CAUTION]
> It will display error image, if the source codes happened **Error** in our FPLAS platform.

<img width="600" alt="setPort" src="https://github.com/lynnhtetaung/flutter-web/blob/docker-deploy/static/error_images/error_image.png">

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 5. Answer File
> Student need to submit 5 exercises' source code under the **Desktop/results/Flutter_CMP_Basic** folder  (e.g. Flutter_CMP_Basic/studentID_Flutter_CMP_Basic_p1.dart in below.)

- ```C://Desktop/results/Flutter_CMP_Basic/studentID_Flutter_CMP_Basic_p1.dart```  at **Windows**
- ```cd Deskop/results/Flutter_CMP_Basic```  at **Linux**
- ```cd Desktop/results/Flutter_CMP_Basic```  at **MacOS**

<a href="#flutter-programming-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 6. Answer File Submission Links & System Usage Feedback
> After finished the exercises, student need to submit answer files of 5 exercises from **studentID_Flutter_CMP_Basic_p1.dart** to  **studentID_Flutter_CMP_Basic_p5.dart** to the Google form **https://forms.gle/BrxTEY87hmqSJQiD6**.
> 
> To submit 5 exercises files are the following format .
- **studentID_Flutter_CMP_Basic_p1.dart** (e.g, 51D27703_Flutter_CMP_Basic_p1.dart)
- **studentID_Flutter_CMP_Basic_p2.dart** (e.g, 51D27703_Flutter_CMP_Basic_p2.dart)
- **studentID_Flutter_CMP_Basic_p3.dart** (e.g, 51D27703_Flutter_CMP_Basic_p3.dart)
- **studentID_Flutter_CMP_Basic_p4.dart** (e.g, 51D27703_Flutter_CMP_Basic_p4.dart)
- **studentID_Flutter_CMP_Basic_p5.dart** (e.g, 51D27703_Flutter_CMP_Basic_p5.dart)

> Please access the following **Google form** for answer file submission and taking survey usage of this system.
  
- 📝 https://forms.gle/BrxTEY87hmqSJQiD6

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">