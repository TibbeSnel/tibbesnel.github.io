# Portfolio Site

#### This project began when I wanted to record my projects in some way. Mostly for myself, so I could look back at the weird stuff I built. But I also wanted to share my projects with the world. So I decided to build a site. 

## How it works
I am not going to explain the whole site here, but here are a few features I'd like to share:

1. First off, the navbar and footer aren't duplicated in code for every separate page, instead they are dynamically loaded into the page. This makes it very easy to make changes to both of them without having to do that for each separate page.
2. The home page carousel and the projects page tiles both load their content via GitHub API, so when I make a new repository or edit the description, it just gets loaded in automatically. Because github API has a rate limit, I wanted to minimize the amount of calls per user, so I added Session Storage for the project titles, descriptions and images. This way all the github data doesn't have to get re-fetched when going to another tab.
3. The terminal (playground page) was a mess to make, it required the most AI because of the javascript. But the result is very cool if I may say so, and there are a lot of easter eggs hidden in it, please try it out if you have some spare time ;). 

## The making
Because I am not planning to become a web developer, I used AI for all the layout and Javascript of the site, but the ideas and contents are mine. Normally I would not use AI to this degree, but in this case I would rather concentrate on learning more fun things than CSS and JS :).

I originally planned to make a separate HTML page for each project, but that would've become repetitive and a pain to maintain. So I tried dynamically loading project data from a JSON file, which actually got pretty far, I had most of it workin, but I eventually realized I was just reinventing Markdown parsing. 

After that, I switched to loading the README.md files directly from each project's GitHub repository and rendering them. That worked, but then I came to the realization that it's a lot easier to link directly to the GitHub repository, so that is what I did.

In the end, I went with a simple approach: the “Projects” tab just links directly to each project’s GitHub page. It’s less fancy, but easier to maintain, and that is far more important.

## What I Learned
Even though this wasn't my favourite project (Anything is better than web development), here's a list, because who doesn't like a list, right?

* Basic HTML, CSS, and JavaScript structuring
* Using fetch() to load remote content
* Working with the GitHub API to fetch README files
* How not to over-engineer something that doesn’t need it
* That Markdown is good actually
* That I definitely don’t want to be a web developer.


