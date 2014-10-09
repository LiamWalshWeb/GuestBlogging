The Skeleton
============

- Intro
    - A little bit of talk about the past of web development
    - How this blog article relates to current/recent work ie The Bookseller micro sites
    - The fact that times have changed and its time for a new approach
- The Core
    - Talk a bit more about the new tools, the Triforce
    - The Triforce - Yeoman, Grunt and Bower
    - Using Yeoman's official webapp generator
- Conclusion
    - Talk about alternatives such as Gulp
    - Mention the more advanced webapp being built by myself
        - Makes use of Assemble, Build Control and other bits
    - Mention the tough bridges to cross etc.
    - Light at the end of the tunnel, harness the power of the Triforce!

The Triforce of Front End Development
=====================================

A lot of the best web developers in the world started off in an era that was witnessing the birth of the internet. The likes of Jeffery Zeldman, `TODO: add more names here` people who are a great influence in the industry and also helped make the web what it is today. I remember reading the blogs and article's that these legends produced and remember the struggles that early web development endured. Long winded and unmanageable CSS files, bloated and unmanageable HTML code and inconsistent Javascript code... that was also unmanageable.

I was born during this time but did not experience the internet till much later in its lifespan in the late 2000's. Joining at a age where the web was going through a transition of which it had never been through before. Responsive web design, preprocessors, code standards, CSS3 and HTML5, these were my first experiences with web development.

The new generation of front enders will face challenges we can't begin to guess but for now this generation must tackle a world wide web that demands bigger better things and with business' cutting to the bone on budgets less time to do so! Fear not for the people have taken up the challenge! The web community is maturing every day and a revolution of open source sharing means new tools are emerging to help with the crisis.

![The Web Triforce](the-web-triforce.png)

> A long, long time ago the web was in an age of Chaos. In the middle of this chaos, on a little website in the realm of The Interent, a legend was being handed down from generation to generation, the legend of the 'Triforce'; three front end tools possessing mystical powers.

## The Revolution

The new revolution of modern web design has brought forth new wonders for the web along with it's challenges and three tools have arisen to help make developers lives better (and to prevent early stress driven graves). These tools include:

- Yeoman -
- Grunt -
- Bower -

Each of these tools tackle a different specific problem but work extremely well together. In Fact Yeoman was designed to work with Grunt and Bower in it's conception. So let's look at a common use case for when you might use these tools.

For The Bookseller company we were asked to create multiple micro-sites such as the Futurebook Conference site, the Marketing and Publicity and the Children's Conference. Each of these sites needed creating with minimal development time and a quick turnaround. None of these sites needed a CMS or anything complicated or dynamic they were purely informational meaning we designed them as simple flat HTML sites.

The first thing a developer might do for a project to go fetch the HTML5 Boilerplate and paste that into an index.html file, go fetch Normalize and paste that into a CSS file or a SASS partial, go fetch Modernizr, jQuery and so on. Tiring stuff right?

![So tired of copy and paste](tired.jpg)

## Yeoman

Yeoman serves as a way to quickly scaffold and put together a website folder structure, pull in dependencies, setup Grunt and Bower files meaning you can be developing a website in minutes! Be rid of the tedious file fetching and web traversing for snippets of code for a basic setup.

For The Bookseller micro-sites we used the official Webapp generator developed by the amazing people behind Yeoman itself! The generator comes with a lot of amazing tools built in for Grunt including SASS and Compass compilation, Autoprefixr, Javascript and Coffeescript concatenation and minification amongst other things. The generator also encorporates Bootstrap and Modernizr as optionals for Bower and even hooks them up!

![Oh my god!!!](omg.gif)

All of this saves time and in turn saves money. The community has taken no time at all in creating they're own generators. Some of my favourite's include `TODO: Favourite's` all of which add to a bigger base of generators to choose from for the right situation.
