---
layout: default
title: "Lining draw"
permalink: Lining-draw
---

# Lining-draw
Processing script that creates shapes from lines only

![](https://img.shields.io/badge/status-Finished-green) ![](https://img.shields.io/github/license/Relex12/Lining-draw) ![](https://img.shields.io/github/repo-size/Relex12/Lining-draw) ![](https://img.shields.io/github/languages/top/Relex12/Lining-draw) ![](https://img.shields.io/github/last-commit/Relex12/Lining-draw) ![](https://img.shields.io/github/stars/Relex12/Lining-draw)



Look it on GitHub:

[![lining-draw](https://github-readme-stats.vercel.app/api/pin/?username=Relex12&repo=lining-draw)](https://github.com/Relex12/lining-draw)

[Read in French.](https://relex12.github.io/fr/Lining-draw)


---

## Summary

* [Lining-draw](#lining-draw)
    * [Summary](#summary)
    * [What is it?](#what-is-it)
    * [What it looks like](#what-it-looks-like)
    * [How to use](#how-to-use)
    * [Code explanation](#code-explanation)
    * [What you can change](#what-you-can-change)
    * [Repository status: Finished](#repository-status:-finished)
    * [Processing compatibility](#processing-compatibility)
    * [Enjoy !](#enjoy-)

<!-- table of contents created by Adrian Bonnet, see https://github.com/Relex12/Markdown-Table-of-Contents for more -->

## What is it?

Lining-draw is Processing project that can draw various shapes from border-to-border lines only.

All you can draw are curves, by increasing or decreasing the coordinates of the lines.

## What it looks like

Here are two examples of pre-recorded figures:

![Capture1](https://raw.githubusercontent.com/Relex12/Lining-draw/master/img/Capture1.PNG)

![Capture2](https://raw.githubusercontent.com/Relex12/Lining-draw/master/img/Capture2.PNG)

## How to use

[Processing](https://processing.org/) is required.

1. Download or clone the repository
2. In the `drawing/` directory, run `drawing.pde`
3. Click the run button to execute

## Code explanation

In the `drawing/` directory, there are three scripts:

* `drawing.pde` is the script you will have to execute, it calls a `figure` function in a switch structure and defines the `step` and `maxVal` values
* `figures.pde` is where are defines all the figures, you can find the basic shape and the four-ray star shape shown above, and a few others, and this is where you are willing to create your own figures
* `fonctions.pde` provides functions for the four up/down left/right corners that are called for every figure

## What you can change

In the `drawing.pde` script, you can modify the size of the result window.  By changing the step value, you change how dense it is filled. The figure variable is only used in the switch that makes you changing the figure quickly.

You can add you own figures in the `figures.pde` script. Make sure you understand how the others work.

## Repository status: Finished

The project was a short one, the author worked alone on this for a short time. The code is given to the GitHub Community for free, only under th MIT License, that is not too restrictive.

If you want to add some features, just fork the repository. There is no plan to accept Pull Requests, but who knows.

## Processing compatibility

As it is a small project, the code has only been tested under Processing 3 (3.5.4). I hope it will work with every older and newer versions.

## Enjoy !
