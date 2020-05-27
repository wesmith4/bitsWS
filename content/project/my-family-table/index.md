---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "My Family Table"
summary: "My individual capstone project for Adjacent Academies"
authors: [admin]
tags: ["web app", "web development", "NodeJS"]
categories: ["Web Apps", "Adjacent Academies"]
date: 2020-05-13T22:00:14-05:00
draft: true
# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter
- name: Site
  url: https://myfamilytable.site
- name: Presentation
  url: https://youtu.be/IyAZ1RIagyI
  icon: youtube
  icon_pack: fab
- name: Slides
  url: https://docs.google.com/presentation/d/e/2PACX-1vSrkfVKZSdl-Dz61Uv6a1hEzp2HKLcAAI_6_xFnzdGXN4rNY-ivbFGOZ6Xrl0YGFtySp0wiHIVYM2cM/pub?start=false&loop=false&delayms=30000
  icon: google-drive
  icon_pack: fab
- name: GitHub
  url: https://github.com/wesmith4/familytable
  icon_pack: fab
  icon: github

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

In mid-March, our Davidson in Silicon Valley program transitioned from our locations on-site in San Francisco to remote learning due to the rising COVID-19 pandemic conditions.  We all experienced very new, unique, and unprecedented living sitations, whether with our families, friends, or other relations.  Despite these unfortunate circumstances, I did find some good in our new situation - I got the opportunity to live at home with my family for an extended period for the first time in a couple of years. One great aspect of living at home was that I got the benefit of all of the home-cooked meals I enjoy so much.

When brainstorming for my individual capstone project, this enjoyment of family recipes and home-cooked meals gave me the inspiration for **My Family Table**.  As I approached the end of my junior year of college, I naturally was thinking to the future, when I would be more independent.  I enjoy cooking, and there have been many times when I texted my mom to ask for a picture of a certain recipe, or live instructions.  I thought to myself, "we should just make an online version of our recipe box" - and then began work on this web app.

## React - a failed attempt
<!-- ![react](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/1280px-React-icon.svg.png) -->

The week before our individual capstone projects, I had begun experimenting with React.js, wanting to learn how to use the framework to create a dynamic frontend for web apps. As I thought about the layout and functionality of My Family Table, I knew that I would need a dynamic form for new recipes - one that would allow users to add and delete input elements for ingredients and steps.  Based on this one need, I decided that I would develop the frontend of My Family Table as a React app. However, as I learned late Tuesday of our project week, this was a big mistake that cost me a lot of time and gave me plenty of headaches.


At that point, I realized that implementing React involves a whole lot more than presenting elements like the ticking clock from the tutorial or the dynamic form from my site.  In order to make React work, I would have to map out the front-end routing by hand in the components - a step I had not researched when first reading up on the documentation.  In the series of projects I worked on during the semester, I did all of the routing with the Express framework, which provides a simple way to manage all *GET* and *POST* requests from the client.  Around 5:00 on that Tuesday, I decided that I was in over my head for a first attempt with React and then scrapped most everything and pivoted to implement my front-end through Express with Handlebars.

## The Pivot
The decision to move away from React meant that I pretty much started over with most of my development.  Aside from the back-end ORM interactions with my PostgreSQL database, I did not have much code that would transfer over.  Knowing how I work best, it made much more sense to start all over with Handlebars views and partials than to attempt to salvage bits and pieces from my React code.

> *"Coding is so much more fun when I somewhat know what I'm doing and can go fast."*

Beginning with my Handlebars `views/` directory, I started with the landing page for new users and the user homepage - both basic pages without any functionality other than anchor tags.  The greater task, however, would be replicate the dynamic form necessary for users to add a new recipe. With React, I could define a component method to add or delete fields for ingredients and steps. I then had to implement those same features with client-side JavaScript.
I accomplished this without too much struggle using JQuery to bind functions for adding and deleting fields to the respective buttons in the form.

<!-- My presentation video on Youtube -->
{{< youtube IyAZ1RIagyI >}}
