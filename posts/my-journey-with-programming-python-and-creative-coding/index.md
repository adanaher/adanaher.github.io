<!--
.. title: My Journey with Programming, Python, and Creative Coding
.. slug: my-journey-with-programming-python-and-creative-coding
.. date: 2024-02-10 10:00:00 UTC-05:00
.. tags: python,creative coding,art,personal
.. category:
.. link:
.. description: My peronal journey with programming, Python, and creative coding as well as what I want this blog to be.
.. type: text
-->

My first exposure to programming was in a computer science course in high school, where we did some very simple programs in C. I then took an introductory CS course in college, where we also used C. I enjoyed both of those courses, but to be honest I didn't really catch the programming bug at that time. I continued my studies in Civil Engineering and commissioned into the Air Force after school, where I did zero programming. It wasn't until I left the Air Force and joined a profesional services company that I started to pick up programming again. I started by doing some scripting in Excel VBA and that turned into working on a web application in [.NET](https://dotnet.microsoft.com/en-us/). That's when my love of programming really took off. While I was doing most of my programming in VB.NET, I was also loving dabbling in other languages, specifically Javascript for web development. This is also when I started looking at Python, which started with reading the great book [_Automate the Boring Stuff With Python_](https://automatetheboringstuff.com/). I wrote a few Python scripts to help automate some processes at work (mostly simple processing of data files and some web scraping). I started a new role a few months later doing mostly data analysis and data science work and the team I was working with used primarily the [R](https://www.r-project.org/) language, so I dug deeply into the R ecosystem and sort of forgot about Python for a few years.

In 2019 I joined a makerspace and started learning about digital fabrication and took a particular interest in laser cutting. I started an art business that year making laser cut art and selling at arts and craft shows around New England. Mostly I was designing my laser cut art in CAD tools like [Autodesk Fusion 360](https://www.autodesk.com/products/fusion-360/overview) using parametric modeling, doing almost no scripting or programming. I also used these CAD tools for dabbling in 3D printing, though I never took to that like I did to laser cutting. At that time, I didn't really think about using my programming skills to create my work until I found that people were using R to make art. I started exploring that some, which eventually led me to [Processing](https://processing.org/) and the Javascript version, [P5.js](https://p5js.org/). These tools excited me because I could both make art that I could digitally fabricate and also make interactive computer-based art. At work I was using R, but when I wanted to write code for fun it was either Processing/Java or Javascript. I always felt like the context switching between different languages hampered my ability to progress as much as I wanted to in my creative coding, but I continued to dabble in both Processing and P5.js.

Fast foward to late 2021, when I started working with a new team at work and we started the process of switching to mostly Python rather than R for our data analysis and data processing tasks. I saw that the most action in the data engineering and data science spaces appeared to be in the Python ecosystem rather than in R (though frankly I still preferred the R Tidyverse syntax to Python's Pandas), so I started really improving my skills in Python. I have been loving that journey digging deep into Python, using it for data science/engineering as well as scripting and building web applications and APIs. I fully agree with the common saying that "Python is the second best language at everything". I have been really enjoying digging deep into Python and seeing all of the exciting developments, including what's happening in the browser with tools like [PyScript](https://pyscript.net/).

I have been using Python pretty extensively for the last couple of years now and am still finding the context switch been writing code in Python during the day, mostly for data analysis, and writing code in Java or Javscript for creative coding after work to be a challenge and a barrier to my creative coding journey. Over the last few years I've been really trying to improve my Python skills further and had been looking for ways to do creative coding in Python, but wasn't really happy with what was available. I had tried using [Processing.py](https://py.processing.org/), a Python mode for Processing that used Jython to interact with the Processing JVM. Jython works with Python 2 and also wasn't supported for Processing 4. I also found it sort of clunky to work with, so it just never stuck.

My creative coding involves making interactive art, like what you might traditionally associate with tools like Processing, as well as creating art that can be plotted using a pen plotter (like the [AxiDraw](https://axidraw.com/)) or CNC tools like a laser cutter. I was really looking for a Python-based environment that would allow me to do projects that fit all of these use cases without having to learn multiple different APIs. A few months ago I started playing with the [Simple Inkscape Scripting](https://inkscape.org/~pakin/%E2%98%85simple-inkscape-scripting) plug-in for Inkscape, which worked fairly well for creating drawings for the pen plotter and for CNC, but didn't really allow for the creation of interactive art like what I could do with Processing. A few months later, I discovered [vsketch](https://vsketch.readthedocs.io/en/latest/) which provides a Processing-inspired API and is purpose-built for pen plotters. I really enjoyed using vsketch and played with it quite a bit, but I was still missing the ability to make interactive art. A couple of months ago I came across [py5](https://py5coding.org/), a version of Processing that uses Jpype and very nicely integrates with the rest of the Python ecosystem. I have been playing with that tool since and have really been loving it. In fact, it's the first and only open source project I've ever financially sponsored. Using it (as well as vsketch) also opened my eyes to other Python tools that could be used in creative coding, such as [Shapely](https://shapely.readthedocs.io/en/stable/).

Since I started my creative coding journey, I've been really intrigued by [digital morphogenesis](https://en.wikipedia.org/wiki/Digital_morphogenesis). That probably started when I read [_The Nature of Code_](https://natureofcode.com/) by Dan Shiffman and the many hours I have spent watching Dan's amazing YouTube channel, [The Coding Train](https://www.youtube.com/channel/UCvjgXvBlbQiydffZU7m1_aw) (seriously, if you've never heard of Dan do yourself a favor and go watch one of his videos. You'll thank me later. I don't think I would have gone as far in creative coding as I have without his infectious energy). Despite my interest in digital morphogenesis, I never felt like I had the skills (or frankly, the patience) to do much more than copy and tweak someone else's code. Now with my improving Python skills, I'm feeling the urge to dig deeper into digital morphogenesis specifically and creative coding in Python more generally. My hope is to document my journey in this blog.

I consider myself a decent Python developer, but by no means an expert in the tools I'm learning for creative coding. My goal with this blog is not to show anyone the one right way of doing anything in Python. In fact, I'm sure there will be things I get wrong. My only hope is to share what I'm exploring so that others can benefit from what I'm learning. I hope to share projects I work on as well as people and things that inspire me along the way. My intention is to focus mostly on creative coding and related technologies, maybe with some interesting data technologies thrown in. To be honest, I don't love writing so my hope will be to keep my posts reasonably short and focused on what I learned or the project I did. I don't plan on having comments on the blog, at least not to start, but if you want to give me any feedback or just connect please feel free to email me at alec@alecdanaher.com.