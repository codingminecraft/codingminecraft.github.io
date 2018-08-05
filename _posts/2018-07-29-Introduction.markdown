---
layout: chapter
title:  "Introduction"
contents: ["Who is this book for", "What prior knowledge is required", "Source content", "Conventions used in this book"]
number: 0
nextChapter: "A Brief Intro To C++"
previousChapter: "Toc"
---
<p class="drop-cap">H</p>ave you ever played Minecraft? If you have, and you're a programmer, then like me you may have thought, "How do you code this?". Well, after about 6 months in the making- and one or two different languages along the way- I have come up with a solution so you don't have too!

Now, some of you may think Minecraft is a simple game that requires very little work, but when you begin to think of all the problems that you must solve, you realize that this game is very difficult indeed! I will highlight a few issues you will run into along the way. Performance, this is a huge issue, be-cause it is very difficult to create a self-generating world that does it quickly. Infinite terrain generation, this brings into the whole idea of a system of saving bits and pieces of the world, loading those bits, and building realistic ter-rain in a *random* fashion. Another problem is the language and engine, I tried Unity... Let's just say, there's a reason we are using Unreal for this. A few more problems you will encounter are biomes, cross-chunk generation of structures, procedurally generating structures and trees, creating an inven-tory and crafting system, and the list goes on.

After that exhaustive little bit on the problems, let me present you with some good news. I've solved these problems for you!

<h3 class="section-title"><a href="#Who-is-this-book-for"><b><i>Section 1--Who is this book for</i></b></a></h3>

So, who is this book for? This book is for anyone who wants to learn how to code Minecraft. This book will teach you how to code it using the Unreal Engine. If you are not familiar with what Unreal Engine is, it is a game engine that does the underlying code for us, that way, we can start coding our game immediately. Some of the areas that Unreal already has coded include: lighting, physics, graphical processing, etc.

<div class="info">
 Notch coded Minecraft entirely from scratch. This means that while we do not need to know how to code the lighting and physics, Notch had to code all of this! This is not an easy task to do.
</div>

The Unreal Engine is a little bit daunting at first. If you have used Unity in the past, then Unreal will quickly become familiar. If you have not used either, Chapter 1 will have a brief overview of Unity.

<h3 class="section-title"><a href="#What-prior-knowledge-is-required"><b><i>Section 2--What prior knowledge is required?</i></b></a></h3>

To complete this book, some prior knowledge would be very helpful. If you do not know how to code at all, then this book is not recommended for you. If you know how to code, but do not know how to code in C++, there will be a brief overview of C++ in Chapter 2. If you already know C++ and how to navigate Unreal Engine, feel free to skip Chapter 1 and Chapter 2.

<h3 class="section-title"><a href="#Source-content"><b><i>Section 3--Source content</i></b></a></h3>

Throughout this book we will be using content that is stored online. I have stored all the content that will be used in this book on Github. You can access the content through this link, <a href="https://github.com/CodingMinecraft-1/Coding_Minecraft">https://github.com/CodingMinecraft-1/Coding_Minecraft</a> . When you click on this link it will take you to a directory called CodingMinecraft. When you click into this directory you will find several other directories called Chapter 1, Chapter 2, etc. Within these directories you will find the answers to the exercises, content that is to be downloaded and more. If I ever refer to online content this is generally the link you will want to go to, unless I specify another link.

So, just to emphasize, any content that is referred to throughout this book can be found online at the link above. I will store each chapter’s progress in the appropriate subfolder. I will typically provide a direct link to the folder. If you are not familiar with Git, Git is an online source control system. This basically means that if you are working on a project you can keep track of changes that you make on Github.com. This is very useful with coding, and if you are not already familiar with Git, I would highly recommend that you familiarize yourself with it. When you are working on a project, if you ever make a mistake that renders your code useless, and you cannot figure out what mistake was made, you can simply revert your project to an earlier version where it was working.

<h3 class="section-title"><a>Section 4--Conventions used in this book</a></h3>

In this book there are different things I would like to point out to the reader from time to time. You have already seen an example of that in the above section. Typically, I will pull out the quote and put a simple description above it. There are four main types of quotes I will have:

<div class="warning">
Watch Out!  This is a warning. I will put this in whenever there is something you should try to avoid, because it can and may cause Unreal to crash. (It’s not a fun process).
</div>

<div class="info">
Want some extra information? These are notes that help but are not necessarily pertinent information to the subject at hand. You can see an example in Section 1 above.
</div>

This book is slightly different than your average textbook. In your average textbook, you typically do not have to worry about conventions surrounding coding. I have placed the most aesthetically appealing style for coding that I can. I try to suit the readers who are reading the black and white print edition, but it also has color for those of you reading the E-Book edition.

If there is some piece of code that we are working on I will typically prefix it with the path, unless it is in the same file. It will look like this:

<div class="code-header">
<< Path/to/file.cpp
</div>
{% highlight c++ %}
void AClass::AMethod() {
	// Some function...
}
{% endhighlight %}

Sometimes, when displaying the code in the book it is not necessary to show the entire sample we are currently working on. If I ever skip some code that is already written I will prefix it with a "⋮" for example

<div class="code-header">
<< Path/to/file.cpp
</div>
{% highlight c++ %}
void AClass::AMethod() {
	// There's some code up here, but I left it out for brevity's sake
		⋮
	// And then I will put the remaining code down here.
}
{% endhighlight %}

That should be all that is needed to introduce the conventions used in this book. Now, I know you are chomping at the bit to get started, so let’s get started!
