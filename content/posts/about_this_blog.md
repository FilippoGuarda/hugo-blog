---
title: "About this blog"
date: 2022-09-12T14:26:30+02:00
draft: true
---

I started working on this blog in August 2022, after a particularly underwhelming exam session. 
Even if I was on holiday, the feeling of guilt resulting from not being able to learn my classes' study topics in a timely manner made it impossible to truly relax. Whatever I did, it felt like time wasted on unproductive things.  
I needed to demonstrate to myself that I could be productive, that I wasn't a slob and that I was able to learn things quickly enough.  
I was also contemplating the idea of making a personal website. 

The web from the 90's always fascinated me, even if I could not experience it first person (I was still sucking my thumb at the time). 
I love the idea of a patchwork of cobbled together personal websites, it seems like a modern-day wild west (I am aware of the dark web, but that's not as accessible and I'd rather stay out of any combination-of-letters-agency's list) compared to the modern monoliths that dominate online traffic.  
The indie web was a cool thing to think about, something that I wanted to be a part of. If not for the sheer commodity of directly owning my content, just for the flair of it. 

These are the circumstances that made me take the decision of building my personal blog, without previuos experience in anything web-related. It wasn't a smart move, but in this case a decision taken on a whim has had very satisfying results. 

## How the blog is made
The first thing I had to learn was how a website worked. I had a vague idea of front-end and back-end dynamics, but I was clueless about hosting, deploying, and actually building a website.  

The first impact was quite frightening to be honest; I had underestimated the complexity of the web, and after a couple hours investigating databases, stacks and web services, it was clear I was underequipped for the task.  
Corners had to be cut, hopefully not too many.

I needed an easy solution for a difficult problem, which usually comes with not solving the problem at all. Fortunately, while browsing youtube (something I started this project with the specific purpose of doing _less_ of) my attention was caught by a [video](https://www.youtube.com/watch?v=ZFL09qhKi5I) recently posted by Luke Smith, a libre-web evangelist and the creator of [landchad.net](https://landchad.net/). He converted me almost instantly to HUGO.

### HUGO was the perfect fit for the task
 
Being an extremely fast static website generator aimed at content generation and management.
Generating a static website solves an incredible amount of problems that a newbie like me would have encountered trying to manage and deploy a dynamic website, some of these are:

1) A static website does **not need a database**: since all the content is stored in a folder structure. This means learning yet another language like php along with database theory is not necessary.  
2) A static website is **inherently more secure**: no backend and no server-side processing means almost no point of contact for attacks. Did I say no database?
3) A static website is **faster**: when you visit this website, all the server has to do is serve you some files, no computing time.  

**But most importantly**

4) It's **cheap a.f.**: At the moment I can host the entirety of the website on GitHub pages at the very convenient price of *free*, and while I bought the domain, keeping the default one was also an option. 

Static websites do have some disadvantages. Usually a dynamic website has some tipe of CMS(content management system) that makes creating and uploading content easier, all the content in a static website has to be hardcoded.  
This disadvantage is negated by the ease of use HUGO brings along. All content only needs to be written in a markdown file, saved in a folder and then compiled with the `hugo` command. Done. 
Another disadvantage of sort is the lack of interaction the user have with a static website. No clicky buttons, no pop-ups, no likes, no comments, no autoplaying videos and machine learning enhanced "you may like" recommendations.  
But the only interaction I want is the reader (you) eyeballs on my text, which has been working out fine with a static. 

The web is chock full of HUGO tutorials, so I will not bother you with yet another one. I have just one piece of advice if you're installing on linux: use [Snap](https://snapcraft.io/install/hugo/ubuntu), source installing does not work and the apt install method has older version at the time of writing. 

HUGO, among other things, lets you install user-made themes. In this way it's possible to avoid styling the website altogeter while mantaining a decent grade of polish if you're not creatively inclined.
In my case I used the wonderful [tale](https://github.com/EmielH/tale-hugo) theme with some adaptations resulting from personal preferences. 

### The hosting choice

As stated previously I opted for hosting my blog on GitHub Pages, as it has a _lot_ of advantages compared to other hosting providers like amazon aws or google.  

First of all, hosting a website on Pages is free, that will always be a plus for a student without budget.  
Secondly, by enabling Actions on the repository that holds the blog file, it is possible to create a separate branch which gets updated at every push; modifying the content of the served website almost instantly and without any further command from the user.

