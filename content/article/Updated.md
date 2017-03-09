+++
date = "2017-01-25T18:40:00-04:00"
title = "New Look - New Feel"
description = "After getting feedback from my peers I decided to update the theme of my blog. This article goes into a bit more detail of the how and why I updated my site's theme"
tags = ["blog", "theme", "fabricator"]
+++
> But little Mouse, you are not alone,
>
> In providing foresight may be vain:
>
> The best laid schemes of mice and men
>
> Go often askew,
>
> And leave us nothing but grief and pain,
>
> For promised joy!
> ***
> ~ Robert Burns: To a Mouse - 1785

### So what happened?

If you have noticed, my last post was back in October, and I said how I had hoped to do quick iterations on my site. Well, that plan backfired when I showed my site to my peers, I received a deal of feedback, the majority being critical. I decided to start from scratch and re-do the theme of my site from scratch.

So what has changed? The color scheme, the layouts, basically everything! One of the processes that I decided to implement this time was to utilize the Pattern Lab style of organization for my theme. I first tried to utilize the node version of Pattern Lab, but I found that there still seemed to be a few things that were still in flux with the codebase. I looked at other style guide generators until finally settling on [Fabricator](https://fbrctr.github.io/).

### What I liked about Fabricator

**Setup** - Getting Fabricator setup within the theme structure of Hugo was as simple as running the command: `npm install fabricator --save` in my theme directory. Fabricator already comes with a directory structure set up to quickly organize your assets, views, and materials (this is Fabricator's method of organization). It made it so that I didn't have to think through the architecture of the theme, it was simply handled for me.

**Configuration** - The documentation that is provided on changing the default structure of Fabricator gave me exactly the direction I needed to implement my own custom version of Pattern Lab. I decided that I would stop at the template level of design as my pages are already being generated by Hugo.

**Template Language** - I found that the use of the HTML file extension just felt right at home with Hugo's template language which is also uses the HTML file extension. The syntax that both use aren't the same, but it was nice not to have to switch back and forth between handlebars and Hugo's HTML templates.

**Fabricators Theme** - I personally love the look and feel of Fabricator's theme for viewing the toolkit styles and I like it just a little bit more than the minimal look and feel of PatternLab's theme. When I got to show off my style guide, it feels more professional.

### What I don't like about Fabricator

**Gulp** - Back when I was a consultant for NorthPoint Solutions, I was gung-ho to use Grunt, and then Gulp. After reading articles however on how to use NPM as a build tool, and even more recently on using webpack to compile assets, I feel like Gulp is a little heavy handed. Each time I run the Fabricator server (yeah it has it's own server) it performs an `npm install` and then runs its compilation task. My thought is to possibly switch to a webpack task on my next iteration of the theme.

**Debugging Tools** - While I don't like PatternLab's theme as much as I like Fabricator's, PatternLab has this nifty tool to switch between small, medium, large, and lastly a 'disco' mode that widens and narrows the viewport so as to see how responsive design is being handled. Now Chrome of course has it's own responsive tool that I made use of, but the ability to quickly see how elements react react when widened and narrowed right from the header of the style guide is a nice feature to have. It would be pretty easy to implement it via Javascript so I might submit a PR with that feature to the Fabricator repository in the future.

### Prologue

I am going to be writing up a tutorial on how I integrated Fabricator with Hugo in due time, but needless to say the set up was fairly straight forward. I was extremely impressed with the flexibility that Fabricator offered me. I was able to create, iterate, and update my style guide with ease. Some of the longer tasks with the new theme wasn't the coding so much as the design and creation of icons and interactive form elements in Illustrator. If you want to take a look at the style guide of my site and see how it all comes together, feel free to check it out [here](https://mealeyst.github.io/macromealey/styleguide).

All the best!