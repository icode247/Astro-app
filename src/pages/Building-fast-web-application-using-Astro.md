---
layout: '../layouts/Header.astro'
---

# Building fast web application using Astro

A static site generator is a tool that generates an entirely static HTML website from raw data and a collection of templates. A static site generator, in essence, automates the job of writing individual HTML pages and makes those sites ready to deliver to users ahead of time.
This tutorial will teach a new static site generator for building fast web applications. You'll create a static blog application using Astro at the end of this tutorial.

Let's get to it.


## What is Astro

Astro is a new static site builder with a robust developer experience that meets light output for the modern web. Astro uses a current server-side templating language that renders directly to HTML & CSS, eliminating heavy JavaScript automatically, and the first site builder to eliminate dead code from your website and only hydrate your basic, interactive UI.

> Note: Astro is still beta software. Therefore, missing features and bugs are expected! The developers are still working towards a stable, production-ready v1.0 release.


## Prerequisites
Ensure you have `Node.js - 14.15.0, v16.0.0, or higher` to get started.


## Scaffold new Project
Let's create a new project with the command below:

```
mkdir my-astro-project && cd $_ 
npm create astro@latest
```

The above command will create a `my-astro-project` folder and prompt for the configuration for the project. Your selection should look like the one on the screenshot below:

![](https://i.imgur.com/bMTgPNQ.png)


After selecting the configuration for your project, change directory into the project directory and start the application with the command below:

```
cd my-astro-site && npm run dev
```

You should the output on the screenshot below on your terminal.

![](https://i.imgur.com/vi9jq3P.png)

Now navigate to `http://localhost:3000/` on your browser. You'd see the Astro welcome as shown on the screenshot below.

![](https://i.imgur.com/WhVt48Y.png)



After going through the prompts in the Astro create command, Astro will create the folder structure below:

📦my-astro-site
 ┣ 📂.git
 ┣ 📂public
 ┃ ┗ 📜favicon.ico
 ┣ 📂src
 ┃ ┣ 📂components
 ┃ ┃ ┗ 📜Layout.astro
 ┃ ┗ 📂pages
 ┃ ┃ ┗ 📜index.astro
 ┣ 📜.gitignore
 ┣ 📜.npmrc
 ┣ 📜README.md
 ┣ 📜astro.config.mjs
 ┣ 📜package-lock.json
 ┣ 📜package.json
 ┗ 📜tsconfig.json
 
 
## Create Components
Let's create our porject component. Before get started, we'll delete the boilerpaltes in our 