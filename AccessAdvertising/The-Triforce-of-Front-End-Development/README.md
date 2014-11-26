The Triforce of Front End Development
=====================================

This article aims at introducing some of the current and most popular tools being adopted by front end developers for building websites and applications for the modern web. We will briefly look at web development years ago and how times have changed, undoubtedly for the better. Moving onto looking at the Yeoman, Grunt and Bower tools and examples of how you can use them to make your workflow more efficient and quality.

A lot of the best web developers in the world started off in an era that was witnessing the birth of the internet. The likes of Jeffery Zeldman, Andy Clarke, Eric Meyer and Ethan Marcotte, people who are a great influence in the industry and also helped make the web what it is today. I remember reading the blogs and article's that these legends produced and have read about the struggles that early web development endured. Long winded and unmanageable CSS files, bloated and unmanageable HTML code and inconsistent Javascript code... that was also unmanageable.

I was born during this time but did not experience the internet till much later in its lifespan in the late 2000's. Joining at a age where the web was going through a transition of which it had never been through before. Responsive web design, preprocessors, code standards, CSS3 and HTML5, these were my first experiences with web development.

The new generation of front enders will face challenges we can't begin to guess but for now this generation must tackle a world wide web that demands bigger better things and with businesses cutting to the bone on budgets, less time to do so! Fear not for the people have taken up the challenge! The web community is maturing every day and a revolution of open source sharing means new tools are emerging to help with the crisis and speed up development time and quality.

![The Web Triforce](the-web-triforce.png)

## The Revolution

The new revolution of modern web design has brought forth new wonders for the web along with it's challenges and three tools have arisen to help make developers lives better (and to prevent early stress driven graves). These tools include:

- [Yeoman](http://yeoman.io/) - A project scaffolding tool
- [Grunt](http://gruntjs.com/) - An automation workflow tool
- [Bower](http://bower.io/) - A package manager tool

All of these tools are command line/terminal applications that require NPM and Node.js. Each of these tools tackle a different specific problem but work extremely well together. In Fact Yeoman was designed to work with Grunt and Bower in it's conception. So let's look at a common use case for when you might use these tools.

For The Bookseller company we were asked to create multiple micro-sites such as the Futurebook Conference, Marketing and Publicity and the Children's Conference sites. Each of these sites needed creating with minimal development time and a quick turnaround. None of these sites needed a CMS or anything complicated or dynamic they were purely informational meaning we designed them as simple flat HTML sites.

The first thing a developer might do for a project to go fetch the HTML5 Boilerplate and paste that into an index.html file, go fetch Normalize and paste that into a CSS file or a SASS partial, go fetch Modernizr, jQuery and so on. Tiring stuff right? Not anymore.

![So tired of copy and paste](tired.jpg)

## Yeoman

Yeoman serves as a way to quickly scaffold and put together a website folder structure, pull in dependencies, setup Grunt and Bower files meaning you can be developing a website in minutes! Be rid of the tedious file fetching and web traversing for snippets of code for a basic setup.

For The Bookseller micro-sites we used the official [Webapp generator](https://github.com/yeoman/generator-webapp) developed by the amazing people behind Yeoman itself! The generator comes with a lot of amazing tools built in for Grunt including SASS and Compass compilation, Autoprefixr, Javascript and Coffeescript concatenation and minification amongst other things. The generator also incorporates Bootstrap and Modernizr as optionals for Bower and even hooks them up! For example simple type these two commands to have a Webapp generator site setup.

    npm install -g generator-webapp
    yo webapp

![Oh my god!!!](omg.gif)

All of this saves time and in turn saves money. The community has taken no time at all in creating they're own generators. Some of my favourite's include [Socketio](https://github.com/individual11/generator-socketio), [Angular Fullstack](https://github.com/DaftMonk/generator-angular-fullstack) and [Style Prototype](https://github.com/north/generator-style-prototype). All of which add to a bigger base of generators to choose from for the right situation.

## Grunt

So with the power of Yeoman we now have a way of getting a project up and running in a consistent and quick way we should look at Grunt! Grunt is a automation tool, think of any menial and boring repetitive task you might go through when developing a website and there is probably a Grunt module that eases the pain.

Common and well known example of repetitive tasks inlcude, compiling SASS/Compass/Coffeescript, minifying of JS and CSS (even as far as HTML!), concatenating files, image optimisation, reloading the browser window and installing third party libraries. Grunt has modules that automate all of these tasks. More uncommon examples and personal favourite modules include [Favicons](https://github.com/gleero/grunt-favicons), [Build Control](https://github.com/robwierzbowski/grunt-build-control), [Uncss](https://github.com/addyosmani/grunt-uncss), [SSH](https://github.com/chuckmo/grunt-ssh), [Google PageSpeed](https://github.com/jrcryer/grunt-pagespeed), [Autoshot](https://github.com/Ferrari/grunt-autoshot) and [Build Control](https://github.com/robwierzbowski/grunt-build-control). For a list of more grunt modules visit the [Grunt offical website](http://gruntjs.com/plugins).

Simply supply the command and away you go!

    grunt serve   // For the webapp will setup a local server with livereload and watch
    grunt build    // Creates a dist folder will all production level assets

![Much boring tasks, such automation, so grunt, much sanity](doge.jpg)

Again this saves valuable development time that would otherwise be spent getting assets ready for production level quality with the potential for human error. These little tasks we do every day add up to a lot of time.

## Bower

Amazing stuff eh? Well now we have everything we could ever need to make our project happen, not quite. It often happens that great libraries such as [Modernizr](http://modernizr.com/), [jQuery](http://jquery.com/), [Animate.css](http://daneden.github.io/animate.css/) and [Normalize.css](http://necolas.github.io/normalize.css/) are missing! Such valuable libraries would go a long way to speeding up and raising the quality of our front end! Never fear, remember our copy paste and manual working days are over. A little birdy told me he can fetch these things for me!

Bower is the front end equivalent of PHP's Composer, Ruby's RubyGems and Node's NPM. All other major programming languages have a package manager of some kind for dealing with integrating and updating third-party packages, something that front end developers have been sorely lacking. No more need to go out and fetch the latest code or wondering which library you also might need included and no more out dating of dependencies.

With one command we can get any popular front end third party library using:

    bower install --save jquery

![Hallelujah!!!](hallelujah.jpg)

What a life saver that is! There is even a Grunt module that comes with the Yeoman Webapp that installs said CSS/JS library directly into your code called [Wiredep](https://github.com/stephenplusplus/grunt-wiredep). This module will turn this:

    <!-- bower:js -->
    <!-- endbower -->

After running this:

    bower install jquery --save

Into this!

    <!-- bower:js -->
    <script src="bower_components/jquery/jquery.js"></script>
    <!-- endbower -->

Magic ;D

## The Future

So there we have a project that fit for the modern web! So many great tools to save time and improve quality of front end production. So what is the future then? If we have these tools now what's the next step?

The year 2013 was the year these tools became known and started to grow interest. 2014 is the year that these tools we really becoming almost industry standards. The popularity of these tools is clear to see, offering much value in exchange for a small learning curve they fulfill a want and need that people may not have realised.

I believe that as the community continues to embrace these tools we will see greater things come forth. To all those who helped made these great things happen, thank you.

![You're awesome!!!](awesome-dog.jpg)
