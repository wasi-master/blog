---
title: 'How I made a website that removes ads, bypassed paywalls for articles'
date: 2022-01-07 10:41:02
tags:
    - projects
category: Instructions
---

Yesterday I built a simple website that takes in a url and removes all ads and paywalled content and you can host it locally. The UI is very nice and pleasing. It uses google's `User-Agent` to pretend it's google and gets the same content that the url would give to google.

<!-- more -->

## Motive

I read a lot of articles, some of them have a paywall. And I don't really want to pay to just read one article. If it was something I use daily then I could consider paying for it but for only once, no. So I usually go to [12ft.io](https://12ft.io) for that but that website doesn't work for New York Times so I wondered if there were any alternatives. Then I thought to myself why wouldn't I be able to make one myself? So here we are now.


## Their Implementation

I first scrolled to the bottom of the [12ft.io](https://12ft.io) page and saw an explanation of how it works:

> The idea is pretty simple, news sites want Google to index their content so it shows up in search results. So they don't show a paywall to the Google crawler. We benefit from this because the Google crawler will cache a copy of the site every time it crawls it. All we do is show you that cached, unpaywalled version of the page.

So it depends on google crawler's cache? Cool. But what if the site isn't cached? I tried it with my own blog and it worked but couldn't show the full page for some reason.

## My Implementation

So they load the cached version of the page the google crawler loaded.
My website pretends to be the google crawler and no caching is required. And it can optionally cache those pages locally and there's no need for google to get involved.

## So how to use it?

You can click the image below to go to the GitHub repo containing the project and in there you'll find instructions on how to set this up and how to use it.

[![wasi-master/13ft - GitHub](https://gh-card.dev/repos/wasi-master/13ft.svg)](https://github.com/wasi-master/13ft)