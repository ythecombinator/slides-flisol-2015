# Uma Introdução a Git & Github

Slides from my talk at Festival Latino Americano de Instalação de Software Livre (FLISOL 2015) about
the importance of versioning and sharing code on Github.

## Tools

These slides are made using [Reveal.JS](http://lab.hakim.se/reveal-js/), [Gulp](http://gulpjs.com/) for
automation, [Jade](http://jade-lang.com/) as a template engine and [Stylus](http://learnboost.github.io/stylus/) 
as a preprocessor. 

## Installing

First of all, make sure you have [NodeJS](http://nodejs.org/) and [GulpJS](http://gulpjs.com/)

Clone this repository:

```sh
$ git clone git://github.com/mabrasil/slides-flisol-2015
$ cd slides-flisol-2015
```

Install NodeJS dependencies:

```sh
$ npm install
```

Run Tasks and Serve:

```sh
$ gulp
```

## Basics

- Each new **slide** (horizontally navigated) is a new `.jade` file in which we work on - and after add in
 `src/templates/index.jade` making the includes in the order of presentation.

- Each new **vertical slide** (vertically navigated, inside a **slide**) is a `section.sec-slide` within the `section`
 in the slide that you're working in.

- Each new **fragment** (that makes elements appear as you navigate inside the slide - giving more interactivity) you
 have to add `.fragment` in the element. Ex.: If you want a list, but you don't want it to be displayed at once, but as
 you navigate in the slide, then you do:

```jade
ul
    li.fragment Item 1
    li.fragment Item 2
    li.fragment Item 3
```

## Thanks

Not made with, but inspired by philosophy behind [this boilerplate](https://github.com/willianjusten/reveal-boilerplate).
