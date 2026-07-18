---
title: এত প্রোগ্রামিং ভাষা কীভাবে মনে রাখি
date: 2022-01-05 00:27:34
---

নতুন প্রোগ্রামিং ভাষা কীভাবে শিখি তা নিয়ে আমার আগের পোস্টটি দেখে থাকলে হয়তো ভাবছেন এই সব প্রোগ্রামিং ভাষা আমি কীভাবে মনে রাখি (বা আদৌ রাখি কি না)। প্রশ্নটা যৌক্তিক, যেমনটা প্রবাদে আছে — *"Jack of all trades and master of none though oftentimes better than master of one"*। আজ ঠিক সেটা নিয়েই আলোচনা করব।

<!-- more -->

## প্রবাদটি সম্পর্কে...

> _Jack of all trades and master of none though oftentimes better than master of one_

উইকিপিডিয়া থেকে: "Jack of all trades, master of none" এমন একজন মানুষকে বোঝাতে ব্যবহৃত হয় যে একটি দক্ষতায় মনোনিবেশ করে বিশেষজ্ঞ হওয়ার বদলে অনেকগুলো দক্ষতায় হাত পাকিয়েছে।

আরও জানতে এই [উইকিপিডিয়া নিবন্ধটি](https://en.wikipedia.org/wiki/Jack_of_all_trades,_master_of_none) পড়ুন।

আমার ক্ষেত্রেও ব্যাপারটা কিছুটা এরকম — আমি অনেকগুলো প্রোগ্রামিং ভাষা জানি কিন্তু Python ছাড়া কোনোটাতে নিজেকে master বলব না। বলতে পারি অন্য ভাষাগুলোয় সাধারণ কাজ করার মতো যথেষ্ট জানি — যেমন Data Types, Variables, Keywords, Logical ও Arithmetical Operators, If else conditions, Loops, Arrays, Functions। কিন্তু শুধু এটুকু জানা আপনাকে কোনো ভাষায় master বানাবে না।

## তাহলে master হতে কী লাগে?

### Standard Library

প্রথম জিনিসটি হলো ভাষাটির standard library আর তা দিয়ে কী করা যায় সেটা শেখা। যেমন [Python standard library-র ডকুমেন্টেশনে](https://docs.python.org/3/library/) ২০০-র বেশি লাইব্রেরি আছে (repl-এ `help('modules')` চালান) আর [node.js-এর built-in মডিউল তালিকায়](https://www.w3schools.com/nodejs/ref_modules.asp) ২৫-এর বেশি। [stringprep](https://docs.python.org/3/library/stringprep.html), [rlcompleter](https://docs.python.org/3/library/rlcompleter.html), [tabnanny](https://docs.python.org/3/library/tabnanny.html), [reprlib](https://docs.python.org/3/library/reprlib.html), [linecache](https://docs.python.org/3/library/linecache.html), [imghdr](https://docs.python.org/3/library/imghdr.html), [fileinput](https://docs.python.org/3/library/fileinput.html), [contextvars](https://docs.python.org/3/library/contextvars.html), [mmap](https://docs.python.org/3/library/mmap.html) — এগুলো এমন কয়েকটির নাম মাত্র যেগুলোর কথা দৈনন্দিন কোডিংয়ে শোনাই যায় না।

### 3rd party লাইব্রেরি

Master হতে আরেকটি জিনিস জানা দরকার — 3rd party লাইব্রেরি, এগুলো ভাষার ডেভেলপারদের অফিসিয়ালি বানানো নয়।

Python-এর জন্য যেমন requests, pylint/flake8/pep8, numpy, pandas, Django/Flask, Pillow, matplotlib

### (প্রায়) যেকোনো কিছু বানাতে পারা

গণিতের মতো অন্য কিছুর ওপর নির্ভরশীল না হলে যেকোনো জিনিস সহজে কোড করতে পারা উচিত।

## আমার কী অবস্থা?

আমি বলব আমি শুধু Python-এ "master", আর কিছুতে আসলে না। অনেক কিছু জানি ঠিকই কিন্তু বেশিরভাগ ক্ষেত্রেই নিজেকে master মনে করি না। তারপরও Python-এ এখনো এমন জিনিস আছে যা জানি না এবং নিয়মিত নতুন কিছু আবিষ্কার করছি। অন্য ভাষার জিনিস ভুলে যাই বলে প্রায়ই Google-এ খুঁজতে দেখি নিজেকে, কিন্তু গুগল করাকে খারাপ চোখে দেখা উচিত না। মূল উদ্দেশ্য তো কিছু একটা বানানো। যেগুলো নিয়মিত ব্যবহার করি সেগুলো মনে থাকে, আর যেগুলো করি না সেগুলো প্রায়ই ভুলে যাই।

> To be able to forget means sanity.
> \- জ্যাক লন্ডন, The Star Rover

## আপনার কী করা উচিত?

তাই কিছু মনে রাখতে চাইলে অনুশীলন করতে হবে। একবার এক মাস Python ব্যবহার বন্ধ রেখেছিলাম, তারপর কিছু জিনিস মনে করার চেষ্টা করতে হয়েছিল আর ভুলে যাওয়ায় গুগল করতে হয়েছিল। Practice makes perfect.
