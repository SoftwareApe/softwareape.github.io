---
categories:
  - Github
  - VSCode
  - Programming
title: "My First VSCode Extension"
date: "2017-11-27T20:14:10+01:00"
draft: false
---

# My first VSCode Extension

I've been using VSCode as my editor of choice for quite a while now. It's a really well-made editor for programmers, featuring many community made high quality extensions.

One of the features I use quite often is multiple selection. You can edit many places at the same time entering the same text. What I was missing however, was an easy to use feature where I could insert a sequence of numbers, for example to do array access.

I searched the extensions, and could only find one extension that kind of qualified. It did however require you to type your sprintf format string on every use. I wanted something easier to use which doesn't distract you from what you're doing.

## VSCode is Electron, Electron is JavaScript

You can't be in the software business without having heard the horrors of JavaScript. Working on embedded systems I hadn't done anything in JavaScript in more than a decade. It couldn't be that hard though.

### Enter the Yeoman Scaffolding Tool.

I looked at the [official tutorial for writing your first VSCode extension](https://code.visualstudio.com/docs/extensions/example-hello-world). They used the [**Yeoman** scaffolding tool](http://yeoman.io/). Working in embedded software I've never seen a system work so well out of the box. You just type in a few short commands and you get your barebones extension with debugging, testing, VSCode workspace and git set up with one simple command.
Also it lets you select TypeScript, which IMHO is much easier than JavaScript, because your editor can help you much better if it knows what interface it's dealing with on a function. So I still didn't learn JavaScript on this adventure. TypeScript isn't half bad though.

### Testing the Extension

Yeoman generated a unit test environment without even asking. It's amazingly helpful to be able to test drive your code right off the bat without having to learn much about a testing framework. Also the VSCode extension skeleton is set up so you can test in a VSCode debugging session in an editor that starts on F5. Pretty amazing!

### Publishing the Extension

#### Writing a Readme

The Readme is what's going to be displayed when you look at the Extension on the Extension marketplace. It's markdown, it doesn't get simpler than that!

#### vsce

I had my code versioned on Github, had used it locally, and now wanted to publish it. Again I was surprised how easy it is. You just need to [install **vsce** and generate a personal token on *Visual Studio Team Services*](https://code.visualstudio.com/docs/extensions/publish-extension). Publishing becomes as easy as typing "vsce publish".

# Conclusion

It took me less than a week, only working a few hours in the evenings after work, to go from knowing nothing about JavaScript and VSCode Extensions to getting my extension it published. Now I know why there's such a plethora of extensions available for VSCode. It has never been easier to extend your editor. The extension is now avaialble on the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=softwareape.numbermonger). If you have an idea, I can only suggest trying it out.