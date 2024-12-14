## Flutter Programmaing Assistant System with Docker

1. ⚙️ [About the System](#1-about-the-system) 
2. 🔨 [Prerequisites](#2-prerequisites) 
3. 🖥 [Follow the procedure according to OS](#3-procedure-according-to-OS) 
	- [Windows](#windows)
	- [Linux (Ubuntu)](#linux-Ubuntu)
	<!-- - [MacOS](#macos)
		- [Intel Processor](#macos-intel-processor)
		- [M1/2/3 Chip Processor](#macos-m-chip-processor) -->
4. 📜 [About Exercises](#4-about-exercises) 
	<!-- - [Exercise-1](#exercise-1)
	- [Exercise-2](#exercise-2)
	- [Exercise-3](#exercise-3)
 	- [Exercise-4](#exercise-4)
  	- [Exercise-5](#exercise-5) -->
5. 📑 [Answer File](#5-answer-file) 
6. 📝 [Answer File Submission & System Usage Feedback ](#6-answer-file-submission-links) 

<hr style="border-top: 2px solid #333;">

## 1. About the System 
<p align="justify"> 
Flutter Programming Learning Assistant System includes frontend, backend and webserver.
<!-- You can see the details of the system user web pages step by step in the link below.
<a href="https://github.com/lynnhtetaung/fplas-2024/wiki/2.-FPLAS-System--Detail" style="font-size: 0.1px; color: #FF0000;">Details </a> -->

</p>

<p align="center">
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>
<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 2. Prerequisites 

|                                                        Tool                                                        | Install | URL                                                                                                     |
| :---------------------------------------------------------------------------------------------------------------------------: | :-------------: | ------------------------------------------------------------------------------------------------------- |
| <img height="50" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/74b958e4-8211-481c-8454-8aa7a719ce8b"> |      Docker       | <ul><li>https://www.docker.com/products/docker-desktop</li></ul>|

- <strong>If necessary,</strong> please download & reference the following user manual 
[fplas_docker.pdf](https://github.com/user-attachments/files/18124457/fplas_docker.pdf) for Docker Desktop.

	
<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 3. Procedure according to OS
- Depending on the Operating System, the way is different. Therefore, please follow the procedure according to the conrrespondence OS.
##

### Windows

> (1) **Get** 3 docker images on the **command prompt(cmd)**.
```
docker pull 24091997/fplas-backend-2024:v1
docker pull 24091997/fplas-nginx-2024:v1
docker pull 24091997/fplas-frontend-2024:v1
```

> (2) **Change** the Desktop directory on the **command prompt(cmd)**.

```
cd Desktop
```

> (3) If have **Git** in your PC, **Clone** the project from Github on the **command prompt(cmd)**. Then, the project directory named **fplas-2024** on your PC's Desktop. 
```
git clone https://github.com/lynnhtetaung/fplas-2024.git
```
Or
> If have no **Git** in your PC, **Download** the project from here
```
[fplas-2024.zip](https://github.com/user-attachments/files/18135141/fplas-2024.zip) , **Move** the project to Desktop and Unzip them.
``` 

> (4) **Open** the **docker-compose.yml** file in the "fplas-2024" and **Modify** the following directory to match your PC's Desktop directory.
```
/home/lynnhtetaung/Desktop/results:/app/addon/output

to

/C:/Users/.../Desktop/results:/app/addon/output (Put your PC Desktop directory in /C:/Users/.../Desktop/)
```

> (5) **Run** the command on the **command prompt(cmd)** to start the Docker containers after modifying.

```
docker compose up
```


> (6) **Open** Chrome browser and navigate to **http://localhost:4000/**

<p align="center">
 <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>


<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

### Linux (Ubuntu)
> **Get** 3 docker images on the **terminal**.
```
docker pull 24091997/fplas-backend-2024:v1
docker pull 24091997/fplas-nginx-2024:v1
docker pull 24091997/fplas-frontend-2024:v1
```

> **Change** the Desktop directory on the **terminal**.

```
cd Desktop
```

> **Clone** the project from Github on the **terminal**. Then, you will see the project directory named **fplas-2024** on your PC's Desktop.

```
git clone https://github.com/lynnhtetaung/fplas-2024.git
```

> **Open** the **docker-compose.yml** file in the "fplas-2024" and **Modify** the following directory to match your PC's Desktop directory.
```
/home/lynnhtetaung/Desktop/results:/app/addon/output

to

/home/.../Desktop/results:/app/addon/output
```

> **Run** the command on the **terminal** to start the Docker containers after modifying.

```
docker compose up
```

> **Open** Chrome browser and navigate to **http://localhost:4000/**

<p align="center">
 <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>

<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

<!-- ### MacOS (Intel Processor, M Chip Processor)
> Apple's transition from Intel processors to its custom-designed chips (M1/2/3), starting with the M1 and subsequent iterations. Before their transition, Apple Mac computers used Intel processors. It is provided for both Intel and M chip processors.
##
> **Get** 3 docker images on the **terminal**.
```
docker pull 24091997/fplas-backend-2024-ios:v1
docker pull 24091997/fplas-nginx-2024-ios:v1
docker pull 24091997/fplas-frontend-2024-ios:v1
```

> **Change** the Desktop directory on the **terminal**.

```
cd Desktop
```

> **Clone** the project from Github on the **terminal**.
```
git clone https://github.com/lynnhtetaung/fplas-2024.git
```

> **Modify** the following directory in the **docker-compose.yml** file (included in the Git clone project on your Desktop) to match your PC's Desktop directory.
```
/home/lynnhtetaung/Desktop/results:/app/addon/output

to

/Users/username/Desktop/results:/app/addon/output
```

> **Run** the command to start the Docker containers after modifying.

```
docker compose up
```

> **Open** Chrome browser and navigate to **http://localhost:4000/**

<p align="center">
 <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="800" />
</p>

<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

-->

## 4. About Exercises
> First, fill **studentID** and click "Go to Exercise" button. 
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page2.png" alt="flutter" width="900" />
</p>

> Choose **Exercise for Flutter Programming**.
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page3.png" alt="flutter" width="900" />
</p>

> Choose **Basic Grammar**. Then, you will see **5** exercises. 

<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page4.png" alt="flutter" width="900" />
</p>

> **Before** finished the exercises, the **remark** will show **Not Started** status. 
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page5.png" alt="flutter" width="900" />
</p>

> **After** finished the exercises, the **remark** will change to the **Completed** status.
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page5-1.png" alt="flutter" width="900" />
</p>

> Select "exercise1". The left side displays **Output in sample source code**, **Expected result** and "Modification guidance". The right side displays **Source Code editor**. 

> Read the **Modification guidance** and modify the source code as same as the **Expected result**.
To see the source code output, click **Run** button.

<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page6.png" alt="flutter" width="900" />
</p>

> **Loading icon** will show during the source code running. It will take a few second to show the result.
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page7.png" alt="flutter" width="900" />
</p>

> If the source code can run successfully, it will show the result in pop-up dialog. Then, click **OK** and see the result.

<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page8.png" alt="flutter" width="900" />
</p>

> If you see 'No Difference Found', your source code is correct and score will get 100%.
Check your latest source code **dart** file for each exercise under Desktop/Flutter_CMP_Basic.

<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page9.png" alt="flutter" width="900" />
</p>

> If you see 'Difference Found', your source code is incorrect and modify the source code again.

<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page10.png" alt="flutter" width="900" />
</p>

> [!CAUTION]
> It will display error image if there is some **Error** in the source code. 

<img width="600" alt="setPort" src="https://github.com/lynnhtetaung/flutter-web/blob/docker-deploy/static/error_images/error_image.png">

<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 5. Answer File
> Student need to submit 5 exercises source code under the **Desktop/results/Flutter_CMP_Basic** folder  (e.g. **Flutter_CMP_Basic/studentID_Flutter_CMP_Basic_p1.dart** in below.)

- ```C://Desktop/results/Flutter_CMP_Basic/studentID_Flutter_CMP_Basic_p1.dart```  at **Windows**
- ```cd Deskop/results/Flutter_CMP_Basic```  at **Linux**
<!-- - ```cd Desktop/results/Flutter_CMP_Basic```  at **MacOS** -->

<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 6. Answer File Submission Links & System Usage Feedback
> After finished the exercises, you need to submit answer files of 5 exercises from **studentID_Flutter_CMP_Basic_p1.dart** to  **studentID_Flutter_CMP_Basic_p5.dart** to the Moodle.
> 
> To submit 5 exercises files are the following format
- **studentID_Flutter_CMP_Basic_p1.dart** (e.g, 51D27703_Flutter_CMP_Basic_p1.dart)
- **studentID_Flutter_CMP_Basic_p2.dart** (e.g, 51D27703_Flutter_CMP_Basic_p2.dart)
- **studentID_Flutter_CMP_Basic_p3.dart** (e.g, 51D27703_Flutter_CMP_Basic_p3.dart)
- **studentID_Flutter_CMP_Basic_p4.dart** (e.g, 51D27703_Flutter_CMP_Basic_p4.dart)
- **studentID_Flutter_CMP_Basic_p5.dart** (e.g, 51D27703_Flutter_CMP_Basic_p5.dart)

> Please access the following **Google form** for answer file submission and taking survey usage of this system.
  
- 📝 https://forms.gle/BrxTEY87hmqSJQiD6

<a href="#flutter-programmaing-assistant-system-with-docker" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">





























<!-- ### FPLAS Interface


1. 📜 [Page 1](#1-page-1) 
2. 📑 [Page 2](#2-page-2) 
3. 🔖 [Page 3](#3-page-3) 
4. 📝 [Page 4](#4-page-4) 
5. 📝 [Page 5](#5-page-5) 
6. 📝 [Page 6](#6-page-6) 
7. 📝 [Page 7](#7-page-7) 
8. 📝 [Page 8](#8-page-8) 
9. 📝 [Page 9](#9-page-9) 
10. 📝 [Page 10](#10-page-10) 


<hr style="border-top: 2px solid #333;">

## 1. Page 1
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page1.png" alt="flutter" width="900" />
</p>

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 2. Page 2
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page2.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 3. Page 3
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page3.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 4. Page 4
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page4.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 5. Page 5
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page5.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 6. Page 6
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page6.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 7. Page 7
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page7.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 8. Page 8
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page8.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 9. Page 9
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page9.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 10. Page 10
<p align="justify"> 
  <img src="https://github.com/lynnhtetaung/fplas-2024/blob/blog/assets/page10.png" alt="flutter" width="900" />
</p>

<a href="#fplas-interface" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

-->
