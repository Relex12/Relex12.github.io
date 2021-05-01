---
layout: default
title: "Dictionaries"
permalink: Dictionaries
---

# Dictionaries

List of dictionaries for Word-Machine

![](https://img.shields.io/badge/status-Up_to_date-green) ![](https://img.shields.io/github/license/Relex12/Dictionaries) ![](https://img.shields.io/github/repo-size/Relex12/Dictionaries) ![](https://img.shields.io/github/last-commit/Relex12/Dictionaries) ![](https://img.shields.io/github/stars/Relex12/Dictionaries)

Checkout on GitHub

[![Dictionaries](https://github-readme-stats.vercel.app/api/pin/?username=Relex12&repo=Dictionaries)](https://github.com/Relex12/Dictionaries)

[Lire en Français](https://relex12.github.io/fr/Dictionaries)

---

## Summary

* [Dictionaries](#dictionaries)
    * [Summary](#summary)
    * [What it is](#what-it-is)
    * [How to use it](#how-to-use-it)
    * [License](#license)

<!-- table of contents created by Adrian Bonnet, see https://Relex12.github.io/Markdown-Table-of-Contents for more -->

## What it is

This repository offers a list of dictionaries that can be used with the [Word-Machine](https://relex12.github.io/Word-machine) word generator.

[![Word-machine](https://github-readme-stats.vercel.app/api/pin/?username=Relex12&repo=Word-machine)](https://github.com/Relex12/Word-machine)

## How to use it

If you have clone both repo in the same parent folder, i.e. you have

```
$ tree
├── Dictionaries
│   [...]
│   └── great-old-ones.txt
├── Word-machine
│   [...]
│   └── word-machine.py
[...]
```

then you can run the following command

`python3 Word-machine/word-machine.py -d Dictionaries/great-old-ones.txt -g 10`

to generate words similar to the names of the Great Old Ones of H.P. Lovecraft's work.

## License

The project is a small one. The code is given to the GitHub Community  for free, only under the MIT License, that is not too restrictive.
