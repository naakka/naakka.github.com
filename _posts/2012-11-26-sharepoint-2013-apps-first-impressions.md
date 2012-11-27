---
layout: post
type: text
title: First Impressions of Developing Apps for Sharepoint 2013
image: /img/sharepoint2013-xtune.png
caption: xTune (hosted on our server on LAMP stack) running inside Sharepoint.
description: Apps are the biggest thing in Sharepoint 2013. It's possible to create Sharepoint apps in just HTML, CSS and JavaScript and even host them on your own server. I have just taken my first steps in developing apps for Sharepoint 2013 and hosting them on a LAMP server. These are my first impressions of the development process.
---

## Background

I code in PHP for a living and I've been a Linux user since 1996. I have zero
experience in .NET, Sharepoint or other Microsoft based development tools. A lot of
our clients use Sharepoint and I was pretty excited when Microsoft announced the Apps
model for Sharepoint 2013. 

With Sharepoint 2013 it should be possible to create apps in a lot of different
technologies including plain old HTML, CSS and JavaScript. It's also possible to
host apps on other servers using any technology you wish. This is what really
peaked my interest as this should make it possible to easily create seamless 
integrations between Sharepoint and any service running, for instance, on a
LAMP stack.

## It's All About the Apps

I guess Microsoft has watched what kind of an ecosystem Facebook has built with
their apps and wanted to do something similar with Sharepoint. I think it's a 
great idea and it's quite promising. 

I have just done some first tests with the development tools and I managed to
write an app that runs [xTune](http://xtune.fi) (running on our server on LAMP stack)
inside Sharepoint. Yes, I know it's not much but it's a start :) 
 

## Poor Documentation

Like I said, I have zero experience in Microsoft development tools or Sharepoint development and
I really had to start from sratch. What struck me the most is the poor quality of the
documentation and tutorials.
Even many open source projects win Microsoft in this regard. Just take a look at
[Symfony](http://www.symfony.com), for instance. Symfony has a excellent documentation
and easy to follow tutorials. I hope this is something that Microsoft
will work on.

The quality of the tutorials is quite poor as well. Just look at the example HTML used in
[this tutorial](http://msdn.microsoft.com/en-us/library/fp142381.aspx).

Yes, you got that right. Using tables and line breaks for a web page layout in 2013. 
I know it's just an example and it's not a big deal
but it doesn't give a very good first impression. If the rest of Sharepoint 2013
is filled with this kind of HTML I would be worried. That was how web sites were made 
15 years ago, it was probably still acceptable 10 years ago but definitely not in 2013. 

## Steep Learning Curve

If you think developing Sharepoint apps will be as easy as creating Facebook apps,
sorry to disappoint you. I've been a Linux user since 1996 and I have zero experience
in Microsoft based development tools or Sharepoint development and, at least for me,
the learning curve seemed to be unnecessarily steep. At least at the moment the poor documentation 
and the lack of proper tutorials and working examples is the biggest obstacle in apps development. 

Maybe my expectations were a bit high. If you've
ever developed Facebook apps, you already know how easy it is. Anyone with a little
knowledge in PHP can write a Facebook app easily. I expected something similar with
Sharepoint apps.



## The Development Tools

<div class="image">
  <img src="/img/sharepoint2013-napa.png" alt="Napa development tools" />
  <p class="caption">The Napa development tool running in Chromium browser.</p>
</div>

Microsoft has released some new web based development tools that should make app 
development even easier. That's good news for anyone who wants to develop apps 
but doesn't want to use Microsoft Visual Studio let alone use Windows. The web based
development tool is called *Napa*. It's actually pretty cool and easy to use.

Sadly, most of the tutorials seem to concentrate on using Microsoft Visual Studio
for developing apps. I'm not sure if the *Napa* tools are usable only for smaller
and simpler apps but either way this is not good. Visual Studio, of course, runs
only in Windows. Developing apps in HTML, CSS and JavaScript should not require
developers to run a certain SDK or OS.

Microsoft is pretty proud that it's possible to develop apps for Sharepoint 2013 using
non-microsoft technologies like plain old HTML, CSS and JavaScript. Sadly, this doesn't
quite work as advertised and it seems that for plenty of things you need to do development
using Microsoft Visual Studio which, of course, requires you to run Windows.


## Final Thoughts

Apps for Sharepoint 2013 are promising and I think this is definitely a step in the 
right direction by Microsoft. But at least at the moment getting started in development
is unnecessarily difficult if you don't have any prior development experience in the
Microsoft ecosystem.  

My biggest complaint is the poor quality and the lack of documentation. But I'm sure
this is something Microsoft will work on before the launch. 

Microsoft seems to
be pretty proud that it's possible to develop apps even if you're not familiar with
Microsoft tools. Sadly, this is not quite true and it seems that for a lot of tasks
you need Microsoft Visual Studio for development and that of course requires you
to run Windows. This is a show stopper for many developers using Mac or Linux. 
If Microsoft wants to attract developers using non-microsoft tools this is something
that they really need to get fixed.