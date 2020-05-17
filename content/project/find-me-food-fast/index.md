---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Find Me Food Fast"
summary: "My very first web app!"
authors: [admin]
tags: ["web app", "web development", "NodeJS", "express"]
categories: ["Web Apps", "Adjacent Academies"]
date: 2020-05-10T07:37:22-05:00

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
  url: http://find-me-food-fast.herokuapp.com
- name: GitHub
  url: https://github.com/wesmith4/find-me-food-fast
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
draft: false
---

## My first web app
"Find Me Food Fast" was the first web app I put online during my Spring 2020 semester learning web development with Adjacent Academies.  As I fiddled around on a Friday in late February with integrating the GitHub repository with "this site called _Heroku_ - have you heard of it?" and putting our then-local app online, little did I know that I was laying the foundation for a workflow I would repeat practically every week for the remainder of the semester.

## How it started
The last week before our spring break during the Adjacent program, we had transitioned from creating static web pages to making _dynamic_ websites (web apps) to accept user input to a server and send/render a response. For our end-of-week project that week, we decided to split into teams a little differently - rather than having the instructors assign groups, we had a _draft_.

Initially, each of the 14 of us was to brainstorm some project ideas, then hone in on just one to present - pitch - to the group.  After the round of pitches from the cohort, we voted on five most popular projects to move forward.  The respective "team captains" of these projects then picked their teammates NFL Draft-style from the rest of the cohort, and we began working furiously on our projects to get a viable product for presentations the next day.

## The Idea
Our meal plan for the semester in San Francisco (tragically cut short by the coronavirus) was, in a word, unbelievable.  With a weekly stipend through the Ritual app, we literally had no choice but to eat each and every meal at restaurants in a city where the variety and quality of food are both top-notch.  There was just one snafu - the app's ability to do complex filters of participating restaurants is somewhat limited.

So, I decided to pitch my idea for a web app that allows users to filter through San Francisco restaurants to find the ones that fit their preferences.  When my idea was chosen by the group, I picked my two team members - Rachel Mclean ([GitHub](https://github.com/rachel-mclean)) and Keith Ng ([GitHub](https://github.com/keithjng)).  This was going to be a short, 1.5 day project, so we got right to work on that Thursday, February 27.

## Development
Aside from this being our first time trying to build a functional web app, we also had to deal with the problem of getting **data** for the site.  After a search, we found a Yelp API that we could call to retrieve SF restaurants by cuisine.  Keith and Rachel took charge of this effort, while I worked on the layout and routing of the site.

When we checked our progress as a group later in the day, we had both a large JSON file with a good number of San Francisco restaurants and a functional site with a structure to allow users to submit their preferences in a form.  The next task, then, was to write a program to read the JSON, filter the data by the user's preferences, and render the results on the page.

## The End result
On Friday morning, we presented our Find Me Food Fast web app to the cohort, showing its functionality to accept user preferences and present the name, address, cuisine, and location of the resulting restaurants from Yelp, complete with mouth-watering photos.

This was a very fun way to start down the road of developing functional web apps, and I am grateful to have worked with awesome teammates!

Visit Find Me Food Fast at https://find-me-food-fast.herokuapp.com !
