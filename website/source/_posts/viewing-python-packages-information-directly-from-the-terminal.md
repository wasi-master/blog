---
title: Viewing python packages' information directly from the terminal
description: How to easily see extensive information about any python package directly from the terminal
---

### Why do I need this?

As a programmer, you probably know how to use a terminal. Sometimes *you just don't want to have to open up a browser* only to check how many downloads your favorite python package has, or you just wanna see how to do something in a specific library such as [django](https://www.djangoproject.com/ "Django makes it easier to build better web apps more quickly and with less code.") or maybe *you want to see if a package exists and see it's description before you install it*. I've also faced these issues so **I went out to create my own library to interface  [PyPI](https://pypi.org/ "The Python Package Index, abbreviated as PyPI (/ˌpaɪpiˈaɪ/) is the official third-party software repository for Python") within a terminal**. 

**I *do not earn nor do I want to earn any gains* from this, this is purely for the users' productivity**

### How does it look?

Here's an example of how the information command looks:

![Image showing how the package info looks](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/qgr3mb9bjz6cwworzvf4.png)

And for the search command:

![Image showing how the package search looks](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hx5ip7cgpgkic5krmj9k.png)

**For screenshots of all the other 15+ commands, be sure to check out [the documentation](https://wasi-master.github.io/pypi-command-line/usage/)**

### How does it work?

How the information command works is that it uses the [PyPI API](https://warehouse.pypa.io/api-reference/json.html "Documentation for PyPI JSON API") to fetch general information about the package. Then it uses the [GitHub API](https://docs.github.com/en/rest/reference/repos#get-a-repository "Documentation page for getting a repo information from the GitHub API") to get information such as the stars, forks, size, etc. Then, at last, it uses the [PyPI Stats API](https://pypistats.org/api/ "PyPI Stats provides Analytics for PyPI packages") to get the download count per month, week, and day. Then it combines all these to form a beautiful display with rich colors, panels, hyperlinks, and much more! It also implements caching logic so usage in long coding sessions can stay smoother than ever!

### How do I install it?

You can install it just by running

```sh
pip install pypi-command-line
```

Then you can use the `pypi -h` command to test it out. For more information **see the [installation page on the docs](https://wasi-master.github.io/pypi-command-line/install/)**

And to test out the package info feature you can run.

```sh
pypi info Django
```

`Django is just, for example, *you can see info for any package on pypi*

### Can I see the source code, please?

The source code is available on GitHub: [wasi-master/pypi-command-line](https://github.com/wasi-master/pypi-command-line)

### Ending Notes

But wait there's more, It has tons of [smart features](https://wasi-master.github.io/pypi-command-line/smart_features/) that help you in many ways, It has [a lot of other commands](https://wasi-master.github.io/pypi-command-line/usage/) too such as [ `browse` ](https://wasi-master.github.io/pypi-command-line/usage/#browse), [ `information` ](https://wasi-master.github.io/pypi-command-line/usage/#information), [ `description` ](https://wasi-master.github.io/pypi-command-line/usage/#description), [ `search` ](https://wasi-master.github.io/pypi-command-line/usage/#search), [ `wheels` ](https://wasi-master.github.io/pypi-command-line/usage/#wheels), [ `releases` ](https://wasi-master.github.io/pypi-command-line/usage/#releases), [ `largest-files` ](https://wasi-master.github.io/pypi-command-line/usage/#largest-files), [ `regex-search` ](https://wasi-master.github.io/pypi-command-line/usage/#regex-search), [ `version` ](https://wasi-master.github.io/pypi-command-line/usage/#version), [ `cache-info` ](https://wasi-master.github.io/pypi-command-line/usage/#cache-info), [ `cache-refresh` ](https://wasi-master.github.io/pypi-command-line/usage/#cache-refresh), [ `cache-clear` ](https://wasi-master.github.io/pypi-command-line/usage/#cache-clear), [ `new-packages` ](https://wasi-master.github.io/pypi-command-line/usage/#new-packages), [ `new-releases` ](https://wasi-master.github.io/pypi-command-line/usage/#new-releases), [ `read-the-docs` ](https://wasi-master.github.io/pypi-command-line/usage/#read-the-docs)
