---
title: 5 python tips that new programmer would love
date: 2022-01-10 00:31:29
tags:
    - tutorial
    - programming
category: Instructions
---

So you're new to python programming? and you want some tips? then you've come to the right place. In this post I'll provide 5 python tips that I see beginners make a lot. And trust me when I say this, I've taught a lot (and I mean a lot!) of people. I've seen a immense range of code ranging from pure beauty to absolute trash.

<!-- more -->

## 1. Follow PEP-8

PEP-8 is a PEP (Python Enhancement Proposal) that suggests coding conventions for python code. Like a style guide for python code. Code is read much more often that it's written, and you should try to make your code as readable as possible, even for you. The guide can be found at [www.python.org/dev/peps/pep-0008/](https://www.python.org/dev/peps/pep-0008/), and you can see a more beautified version at [pep8.org](https://pep8.org)

## 2. Ask good questions

In your journey you'll often get stuck doing something. Especially if you try to code by yourself. In this situation you might want to search online for solutions first. Then if there aren't any solutions you may be tempted to ask someone, maybe in a Discord server, maybe some friend you know that does programming. In any case, you should always ask good questions, there is a [great guide from stackoverflow](https://stackoverflow.com/help/how-to-ask) that'll help you with this. And don't ask a [XY problem](https://xyproblem.info/)

> A prudent question is one-half of wisdom.
> \- Francis Bacon

## 3. Don't do `import *` or `from … import *`

Now at first you may think, importing everything makes it so easy, less typing, less hassle. But let me stop you right there. This may seem like it'll make it easy, but you'll regret it later down the line. Doing this makes it hard to figure out which functions are import (and from where), and which functions are custom defined. It also makes it hard for 3rd party tools like `pyflakes` to do static analysis with your imports. This WILL import a lot of stuff you'll never use and will clutter up the namespace. As a concrete example, many users of NumPy have been bitten by `numpy.any` shadowing `any` when they do `from numpy import *`. According to the Zen of Python:
> Explicit is better than implicit.

[And even the official documentation for python discourages this](https://docs.python.org/3/tutorial/modules.html#:~:text=note%20that%20in%20general%20the%20practice%20of%20importing%20*%20from%20a%20module%20or%20package%20is%20frowned%20upon%2C%20since%20it%20often%20causes%20poorly%20readable%20code.%20however%2C%20it%20is%20okay%20to%20use%20it%20to%20save%20typing%20in%20interactive%20sessions.)

## 4. Read the documentation

Beginners, especially people whose native language is not English, don't really want to read the documentation on stuff. Now this can be a very bad thing. You should always use what's given to you. Reading documentation could bring out details you never could have otherwise found out. If you can't find anything in the documentation you might also want to look at the source code. But the main thing is you should learn to read the documentation. If your English is weak then you may want to use [Google Translate's website translation tool](https://support.google.com/translate/answer/2534559)

> The more that you read, the more things you will know. The more that you learn, the more places you'll go.
> \- Dr. Seuss

## 5. Always following tutorials

Tutorials can be good, tutorials can be bad. Specially in the case of programming. There are always more than one way to do things and if a tutorial shows a way that is bad then you'll learn it and remember it thinking it is really good but in reality it was not that good. Always research on your own first, I've seen countless outdated tutorials that show stuff that used ot exist but don't exist anymore, see if the tutorial you're watching is recent or not. And try not relying on tutorials too much since you want to make stuff yourself and not be taught like a puppet what to do. In the real world there won't be a guide you can just follow and everything would be done just by itself

> No one achieves great things by following the crowd. Have a spine. Strike your own path.
> \- Robert Kiyosaki

> It's easy to stand with the crowd, it takes courage to stand alone.
> \- Gandhi
