---
title: 'HCI Lab 1'
description: 'First lab in Human-Computer Interaction'
pubDate: 'Sep 25 2023'
heroImage: '/blog-placeholder-1.jpg'
---

Hi everyone !

Last friday during my first lab, I learned with the help of a fellow student, <a href="https://thibaultellong.github.io"> Thibault Ellong</a>, how to make a blog with <a href="https://astro.build"> astro.build</a>, and how to deploy it with GitHub. A week before that I had also learned during my Computer Graphic Class, how to setup a Unity project.

#### 1. Building this blog

This is my very first time creating a blog. To chose a good static site generator I followed the advice of my comrades and started to build with Astro.

The first thing I had to do was to install Node.js and npm on my computer. Do it with <a href="https://nodejs.org/en/download"> this site </a>.

Now, after creating a folder on your device where all your work will be, you can chose the template you want on <a href="https://astro.build/themes/"> astro website </a>.
Open a terminal and place yourself in your previously created folder (careful about that, I made the mistake and I had to change everything by hand afetrward). Now you can create you new project with npm :
```
mkdir your_local_project_folder
cd /your_local_project_folder
npm create astro@latest
```

It's now, time to create your github repository to be able to update your website in the future. For that follow the steps on the <a href="https://pages.github.com"> github website</a>.
Name your repository <username>.github.io

Now you go back to your terminal, in your folder and you can clone your repository and update your files :

```
cd /your_local_project_folder
git clone https://www.github.com/<username>/<username>.github.io.git
git add * 
git commit -m "first commit"
git push
```

Now go in the astro.config.mjs file in your project and suppress everything to replace it with this block :
```
import { defineConfig } from 'astro/config'
export default defineConfig({
  site: 'https://<username>.github.io',
})
```
In you project, you should now create a file **.github**, then inside a file **workflow** and inside a file **deploy.yml**

All left for you to do now is to follow <a href="https://docs.astro.build/en/guides/deploy/github/">this tutorial</a> to deploy your Astro site to Github Pages.


#### 2. First steps with Unity

During the first week of my class, I was introduced to Blender and Unity, which opened up a new realm of possibilities for me. I'll be sharing the projects I have planned in a future post, but for now, let's focus on my initial experiences with Unity and some essential knowledge that I've gathered, especially for beginners like myself.

Unity, I discovered, is a robust game development engine that offers a lot to learn. Of course choosing an engine when developping your own game depends before anything of your needs. 

Here are some practical insights that can help beginners like me get started:

1. **Getting Familiar with the Interface**: Unity's interface can be a bit overwhelming initially. Take some time to explore the various panels, tabs, and windows. Becoming comfortable with the interface layout will make your journey smoother. The very first thing I learned was how the interface was devided between the different windows : 



2. **Understanding Game Objects**: In Unity, everything revolves around game objects, whether they're characters, scenery, or interactive elements. Learning how to create and manipulate these game objects is fundamental.

3. **Working with Components**: Game objects come to life through components. Components are scripts or properties that define an object's behavior, appearance, and interactions. Understanding how to attach and customize components is key to creating dynamic experiences.

4. **Utilizing the Asset Store**: Unity provides an Asset Store with a vast library of pre-made assets, scripts, and templates. This resource can save you significant time and effort as a beginner.

5. **Scripting (Optional)**: Learning to script in C# or Unity's scripting language, UnityScript (similar to JavaScript), can give you more control over your projects. It's not necessary for every project, but it's a valuable skill to develop.

6. **Collaboration Tools**: If you're working on projects with others, Unity's collaboration tools are essential. They enable efficient teamwork, version control, and project management.

7. **Documentation and Community**: Unity has a helpful community of developers and comprehensive documentation. When you encounter challenges, don't hesitate to consult forums, tutorials, or the official documentation – chances are, others have faced similar issues.

As a beginner, I'm excited to continue my journey into Unity, and I invite you to come along with me. In the upcoming posts, I'll share my progress, projects, and insights as we delve deeper into the world of game development with Unity. Stay tuned for more practical advice and experiences!

Here are some links to help yoou get started and which helped me writing this post 
https://hub.packtpub.com/what-you-should-know-about-unity-2018-interface/