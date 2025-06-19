# React
***
React is a JavaScript library for building frontend user interfaces, especially for single-page applications (SPAs). It runs in the browser and helps manage the visual and interactive parts of a website.

## Sometimes things happen on their own
Don’t stress about having the perfect environment—bad setups and messy code are part of the process.
Just go for it: write, download, build.
I used to tell people do not download anything not familiar with, but looking back, that was a big mistake caused by a misunderstanding.

**How to download react and connect vite and Http**  
https://high-career.jp/2022/01/04/vscode-react-dev/  
https://zenn.dev/longbridge/articles/93f63e0423785b  
https://zenn.dev/longbridge/articles/82194eb0eaf710

**Tips**  
1.If you're downloading something using ***cmd*** and want a specific version, simply add the version number after the package name.  
2.After creating a project, dependencies are typically installed locally (inside the project folder). Be sure to verify them in the node_modules directory or check the package.

## Why Isn't React Development as Visual as Eclipse

### Introduction
As someone used to developing in Java and Spring using Eclipse, I was genuinely puzzled when I started learning React:

Why doesn’t React development come with a fully visual IDE like Eclipse? --> First,download node.js and npm will be downloaded at same time! Second even npm was down at same time still need to install.
Why does everything seem to require the command line (CLI) and configuration files?

This blog post is a summary of what I learned as I transitioned from backend Java to frontend React.

### The Core Differences Between React and Java Ecosystems
**Spring Boot is a Full Platform; React is Just a UI Library***

Spring Boot handles everything—MVC, REST APIs, databases, scheduling, security, and more.

React only focuses on the user interface (UI) logic. Everything else—like routing, state management, and API integration—is up to myself.

With React, I decide whether to add tools like React Router, Redux, TailwindCSS, Axios, etc.

| Aspect |Java / Spring (Eclipse) |React (Node.js Ecosystem)|
|----------|----------|----------|
|Project Management|Maven / Gradle (structured)|npm / yarn (modular, dynamic)|
|Build Tool|Maven lifecycle|Vite / Webpack / Rollup|
|Workflow|Visual IDE (buttons & menus)|CLI + lightweight editors (e.g., VS Code)|
|Project Start|Click "Run"|npm run dev|
|Configuration|	pom.xml|package.json|

### The Relationship about Node.js,Npm,Create-react-app,Vite,Create,React and VSCode

* Node.js: Like the “stove” in your kitchen — without it, you can’t cook (run) your raw ingredients (JavaScript code).

* Npm: Your “spice cabinet,” where you keep all kinds of spices (third-party libraries and packages) to add flavor to your dishes (projects).

* React: The “signature dish” you want to cook — a popular recipe for building beautiful and interactive user interfaces.

* Create-react-app (CRA): Like a “semi-prepared meal kit” that provides all the ingredients and tools so you can start cooking your signature dish right away. It uses the “traditional stove” (Webpack) and defaults to burner number 3000 (local port).**It's been phased out by time.**

* Vite: A new-generation “smart induction cooker,” faster and more efficient, with its own meal kits to help you cook React dishes quicker. It defaults to burner number 5173.

* Create: The action of “calling ‘start cooking!’” — telling the kitchen to begin cooking with a certain meal kit, such as npm create vite or npx create-react-app.

* VSCode: Your “kitchen console” equipped with knives, cutting boards, an artillery control panel, recipes, and timers (plugins, debugging tools, smart suggestions, etc.) that make your cooking (coding) smoother and more efficient.

### The different between VScode ternimal(PowerShell) and CMD  
* PowerShell is a more powerful command-line interface (CLI) compared to the traditional CMD (Command Prompt). It supports advanced scripting, automation, and system management tasks.  

* In modern Windows environments, PowerShell is the default terminal in many tools—including Visual Studio Code (VSCode)—because of its enhanced capabilities and active development by Microsoft.  

* However, PowerShell enforces a security policy called Execution Policy. This limits the execution of untrusted or unsigned scripts to protect users from running potentially harmful code.

* In contrast, CMD does not enforce script execution policies, making it more permissive but less secure. This is why many beginners switch to CMD when encountering PowerShell restrictions.

* Can switch terminal types in VSCode from the dropdown menu in the terminal panel and choose CMD, Git Bash, or PowerShell depending on your needs.




A Java Developer’s Perspective on Front-End Workflow
Author: A Java-turned-frontend beginner × ChatGPT
Date: June 2025
