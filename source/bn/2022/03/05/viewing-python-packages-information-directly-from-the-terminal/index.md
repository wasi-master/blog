---
title: Python প্যাকেজের তথ্য সরাসরি টার্মিনাল থেকে দেখা
date: 2022-03-05 00:00:00
description: যেকোনো Python প্যাকেজের বিস্তারিত তথ্য সরাসরি টার্মিনাল থেকে সহজে দেখার উপায়
---

### এটা আমার কেন দরকার?

প্রোগ্রামার হিসেবে টার্মিনাল ব্যবহার আপনি নিশ্চয়ই জানেন। কখনো কখনো *শুধু ব্রাউজার খুলতে ইচ্ছা করে না* — হয়তো দেখতে চান আপনার প্রিয় Python প্যাকেজের ডাউনলোড কত, বা [django](https://www.djangoproject.com/ "Django makes it easier to build better web apps more quickly and with less code.")-র মতো কোনো নির্দিষ্ট লাইব্রেরিতে কোনো কাজ কীভাবে করে তা দেখতে চান, বা *কোনো প্যাকেজ আদৌ আছে কি না আর ইনস্টলের আগে তার বিবরণ দেখতে চান*। আমিও এই সমস্যাগুলোর মুখে পড়েছি, তাই **টার্মিনালের ভেতর থেকেই [PyPI](https://pypi.org/ "The Python Package Index, abbreviated as PyPI (/ˌpaɪpiˈaɪ/) is the official third-party software repository for Python")-র সাথে কাজ করার জন্য নিজের একটি লাইব্রেরি বানিয়ে ফেলেছি**।

**এ থেকে আমি *কোনো আয় করি না, করতে চাইও না*, এটা পুরোপুরি ব্যবহারকারীদের প্রোডাক্টিভিটির জন্য**

### দেখতে কেমন?

Information কমান্ডটি দেখতে যেমন লাগে তার একটি উদাহরণ:

![প্যাকেজ info দেখতে কেমন তার ছবি](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/qgr3mb9bjz6cwworzvf4.png)

আর search কমান্ডের জন্য:

![প্যাকেজ search দেখতে কেমন তার ছবি](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hx5ip7cgpgkic5krmj9k.png)

**বাকি ১৫+ কমান্ডের স্ক্রিনশট দেখতে অবশ্যই [ডকুমেন্টেশনটি](https://wasi-master.github.io/pypi-command-line/usage/) দেখুন**

### এটা কাজ করে কীভাবে?

Information কমান্ডটি প্রথমে [PyPI API](https://warehouse.pypa.io/api-reference/json.html "Documentation for PyPI JSON API") ব্যবহার করে প্যাকেজের সাধারণ তথ্য আনে। তারপর [GitHub API](https://docs.github.com/en/rest/reference/repos#get-a-repository "Documentation page for getting a repo information from the GitHub API") ব্যবহার করে star, fork, size ইত্যাদি তথ্য নেয়। সবশেষে [PyPI Stats API](https://pypistats.org/api/ "PyPI Stats provides Analytics for PyPI packages") থেকে মাস, সপ্তাহ ও দিনপ্রতি ডাউনলোড সংখ্যা আনে। তারপর এসব একসাথে জুড়ে rich রং, প্যানেল, হাইপারলিংক আর আরও অনেক কিছু দিয়ে একটি সুন্দর প্রদর্শনী তৈরি করে! এতে caching লজিকও আছে যাতে দীর্ঘ কোডিং সেশনে ব্যবহার আরও মসৃণ থাকে!

### ইনস্টল করব কীভাবে?

শুধু এটুকু চালিয়েই ইনস্টল করতে পারবেন

```sh
pip install pypi-command-line
```

তারপর `pypi -h` কমান্ড দিয়ে পরখ করে দেখতে পারেন। আরও তথ্যের জন্য **[ডকুমেন্টেশনের ইনস্টলেশন পেজ](https://wasi-master.github.io/pypi-command-line/install/) দেখুন**

আর প্যাকেজ info ফিচারটি পরখ করতে চালান:

```sh
pypi info Django
```

Django এখানে শুধু উদাহরণ, *PyPI-র যেকোনো প্যাকেজের তথ্য দেখতে পারবেন*

### সোর্স কোডটা কি দেখা যাবে?

সোর্স কোড GitHub-এ আছে: [wasi-master/pypi-command-line](https://github.com/wasi-master/pypi-command-line)

### শেষ কথা

আরে দাঁড়ান, আরও আছে! এতে টনকে টন [স্মার্ট ফিচার](https://wasi-master.github.io/pypi-command-line/smart_features/) আছে যা নানাভাবে আপনাকে সাহায্য করবে, [আরও অনেক কমান্ডও](https://wasi-master.github.io/pypi-command-line/usage/) আছে যেমন [ `browse` ](https://wasi-master.github.io/pypi-command-line/usage/#browse), [ `information` ](https://wasi-master.github.io/pypi-command-line/usage/#information), [ `description` ](https://wasi-master.github.io/pypi-command-line/usage/#description), [ `search` ](https://wasi-master.github.io/pypi-command-line/usage/#search), [ `wheels` ](https://wasi-master.github.io/pypi-command-line/usage/#wheels), [ `releases` ](https://wasi-master.github.io/pypi-command-line/usage/#releases), [ `largest-files` ](https://wasi-master.github.io/pypi-command-line/usage/#largest-files), [ `regex-search` ](https://wasi-master.github.io/pypi-command-line/usage/#regex-search), [ `version` ](https://wasi-master.github.io/pypi-command-line/usage/#version), [ `cache-info` ](https://wasi-master.github.io/pypi-command-line/usage/#cache-info), [ `cache-refresh` ](https://wasi-master.github.io/pypi-command-line/usage/#cache-refresh), [ `cache-clear` ](https://wasi-master.github.io/pypi-command-line/usage/#cache-clear), [ `new-packages` ](https://wasi-master.github.io/pypi-command-line/usage/#new-packages), [ `new-releases` ](https://wasi-master.github.io/pypi-command-line/usage/#new-releases), [ `read-the-docs` ](https://wasi-master.github.io/pypi-command-line/usage/#read-the-docs)
