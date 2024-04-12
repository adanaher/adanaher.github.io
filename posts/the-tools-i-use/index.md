<!--
.. title: The Tools I Use
.. description: A summary and review of the tools I use to make my laser cut wood art
.. slug: the-tools-i-use
.. date: 2024-04-10 21:19:14 UTC-04:00
.. tags: laser cutting,3d printing, plotting,lightburn,rhinoceros
.. category:
.. link:
.. type: text
.. thumbnail: {{% thumbnail "/images/20240412_140056.jpgg" %}}{{% /thumbnail %}}
-->

I often get asked at art shows how I make my art. I'm often the only artist there using digital fabrication, so I suspect many people haven't seen work like mine before. While I get excited describing how I make my art, I wanted somewhere to point people for a more detailed explanation of my process and the tools I use, so this post is the result. I ended up going into a lot of detail than expected while writing, so this may be geared more towards people who are interested in making art like mine rather than those who are just curious. Hopefully you'll find value no matter which group you fall into.

<!-- TEASER_END -->

<figure>
    <img src="/images/20240412_140056.jpg"
         alt="Laser cutter in my workshop">
    <figcaption>My un-Instagram worthy workshop</figcaption>
</figure>

My methods for making my art have evolved in the 5 years I’ve been doing it. I leverage a mix of skills from various disciplines, using CAD skills that I learned in engineering school, programming skills that I have picked up in my career, and "maker" skills that I have picked up along the way.

I started making my art in 2019 at <a href="https://makersworkshop.com/" target="_blank">Makers Workshop</a>, a makerspace in Maynard, Massachusetts. I joined the makerspace without any grand dreams of embarking on a new hobby/side hustle/art practice. I had never laser cut or 3D printed a thing in my life, but have always loved technology and building stuff, so it seemed like something I wanted to explore. I learned the various tools and tried them all, but for whatever reason the laser cutter drew me like a moth to flame.

# Laser Cutter

After about 9 months of making my art and monopolizing the laser cutter at the makerspace, I decided to get my own laser cutter. I tried doing research to find the “best” one, but it’s such a specialty tool that there wasn’t a ton of information out there. I landed on the <a href="https://lagunatools.com/cnc/co2-lasers/smartshop-laser-mx/" target="_blank">Laguna SmartShop Laser MX</a>, not because my research told me it was the best, but because it seemed like a good enough option. Do I think it was necessarily the best choice now in retrospect? No, but I’ve been happy with the laser and don’t have much to compare it to. It was one of the more affordable options and I wasn’t looking to spend an arm and a leg since I wasn't really sure if I would even be able to sell enough work to recoup my costs (I eventually did). Overall, I have been happy with it and don’t have any complaints. If I could go back and do things differently, probably the only thing I would change is getting the EX model, which has a larger bed and can therefore cut larger pieces.

If you’re looking for a laser of your own, I think the Lagunas are a solid choice (there are a few different bed sizes available in the series). I recommend you do your own research and see what you think, but if you’re at a loss for what to get and are overwhelmed by the choices available, I don’t think you’ll be disappointed with the Laguna.

# LightBurn

While I'm happy with my laser cutter, I’m slightly more willing to gush about the software I use to drive the laser. The default laser cutter software that comes with Ruida controllers (the controller in the Laguna and many other laser cutters) is RDWorks, which I don’t think I ever even used. The makerspace was using a software called <a href="https://lightburnsoftware.com/" target="_blank">LightBurn</a>, which is compatible with many different types of laser controllers, including Ruida. I bought and started using LightBurn almost immediately and am very happy with it. It’s obvious that whoever created this software understands the needs of the laser cutting community and also knows how to design good software. I gladly pay my $30 every year to renew my software license. If you have a laser cutter with a controller compatible with LightBurn, I highly recommend using it.

Another thing that took me far too long to do was to get the <a href="https://lightburnsoftware.com/products/lightburn-bridge-kit" target="_blank">LightBurn Bridge</a>. I used to have to carry my laptop running LightBurn into my dusty workshop and connect to the laser with USB every time I wanted to start a cut. As a result, my laptop got pretty dirty and I think I've done permanent damage to the cooling fan. The LightBurn Bridge changed that. I bought the kit from LightBurn, which included a small Raspberry Pi computer loaded with the LightBurn Bridge software. I simply plugged in the Raspberry Pi and connected it to the laser via ethernet and then did some setup on my computer and voila, now I can send my cuts directly to the laser from my computer without lugging my laptop into the workshop. It’s been a game changer for me.

# Drawing Tools

While LightBurn allows you to do some creation and editing of geometry, I tend to use other software to do my design work and then use LightBurn to clean up the design and prepare it for cutting. I started by using <a href="https://www.autodesk.com/products/fusion-360/overview" target="_blank">Autodesk Fusion 360</a> for my design work, mostly because it was free for hobbyists and I had used AutoCAD and Autodesk Inventor in college, so I understood how CAD software worked and specifically how Autodesk’s products worked. I moved away from Fusion 360 after a few years because they changed their licensing and I was going to have to start paying a hefty subscription fee, which wasn't worth it to me. I also found it crashed on me often while I was sketching, causing me to lose work. I was starting to become interested in parametric design and how that could play into my art and I kept seeing <a href="https://www.grasshopper3d.com/" target="_blank">Grasshopper</a>, a visual parametric design tool for <a href="https://www.rhino3d.com/" target="_blank">Rhinoceros</a>, all over the place and that was enough to get me to make the switch to Rhinoceros. I am overall very happy with Rhinoceros and Grasshopper. I go through phases where I don’t use them much and then there is a slight learning curve to get back into them, but overall they are great software and have a good community behind them.

Many other artists who do work like mine seem to primarily use vector graphics software, most commonly <a href="https://www.adobe.com/products/illustrator.html" target="_blank">Adobe Illustrator</a>. I haven’t used Illustrator before, but have used <a href="https://inkscape.org/" target="_blank">Inkscape</a>, a free and open source vector graphics software that is similar to Illustrator, for some of my designs. In general, the way my brain works seems to align more with CAD software, so that is what I tend to prefer over vector graphics software. I would probably be very happy in something like Illustrator eventually, but I suspect there would be a learning curve to get me there and I’m happy in Rhinoceros. If it ain't broke, don't fix it.

Most of my designs are some combination of manual drawing within Rhinoceros and algorithmic geometry using Grasshopper. The makers of Rhino and Grasshopper do a good job allowing you to combine these two approaches relatively seamlessly. One thing I haven’t explored as much as I would like is using Python within Rhinoceros and Grasshopper. One thing that has stopped me up until now is the fact that before the current version of Rhinoceros, Rhino 8, the Python scripting used a very outdated version of Python that relied on IronPython and didn’t allow using most external libraries, which I felt would limit its utility to me. Rhino 8 added support for CPython (the most common Python implementation) and therefore allows the use of Python 3 and external libraries. It also has an updated <a href="https://www.rhino3d.com/features/developer/scripting/#refreshed-editor--new-in-8-" target="_blank">script editor</a>, which seems like it will improve the developer experience for using Python in Rhinoceros. I missed the window for the discounted upgrade (because I hadn’t learned about the Python update yet) and so am holding off on pulling the trigger to update my software.

# Generative Art Tools

In addition to Rhinoceros and Grasshopper, I often create some designs using generative approaches in <a href="https://processing.org/" target="_blank">Processing</a>, <a href="https://p5js.org/" target="_blank">p5.js</a>, and most recently <a href="https://vsketch.readthedocs.io/en/latest/index.html" target="_blank">vsketch</a> and <a href="https://py5coding.org/" target="_blank">py5</a>. I use Python at work and found it challenging to context switch between Python and Java or Javascript and I found it hampered my ability to express myself. Once I found some generative tools in Python I started using those much more. I intend to write a lot more about my adventures in generative art in the future, so I'll keep this section short for now.

# Other Stuff

In addition to laser cutting, I also dabble in a few other digital fabrication tools. I have a 3D printer, a <a href="https://www.prusa3d.com/" target="_blank">Prusa</a> i3 MK3S, and an <a href="https://axidraw.com/" target="_blank">AxiDraw</a> pen plotter. The 3D printer doesn’t really factor into my art much, but I also like to play with electronics and I occasionally use that to support that exploration. I'm exploring making more art with my AxiDraw, but I also kind of like keeping that as a part of my art practice that isn't driven by commercial interests.

I hope this gave you a little insight into the tools I use. I intend to write a post in the future with recommendations about how to get started making laser cut art, but in the meantime if you have any questions about my process or would like any recommendations about how to get started yourself, feel free to reach out via email or social media.
