---
layout: post
title:  "Intro to basic html"
date:   2014-12-18
categories: intro
---

A few notes
-----------

I'm going to cover as much as I can and start from the absolute basics. I'm sure you already know some of it, if not many of it, but I'll just cover as much as I can to be on the safer side. And chances are I'll miss a fair bit too, so feel free to IM/email me and I'll add to it.

Some useful sites
-----------------

[W3schools][w3schools] is a good place to start if you hit any roadblocks. It's not always accurate and can sometimes be outdated, but for basic stuff like HTML it's fairly reliable. Its CSS section can be questionable at times, but still fairly usable.

Frequently used tags
--------------------

HTML uses tags, and tags are those little words between <> that helps us shape and define the pages. Some tags require to be opened and closed while others do not. Opening a tag is as simple as writing it out, and closing it is adding a / in it at the end. An example would be...

{% highlight html %}

<p> Boom, example time. </p>

{% endhighlight %}

The only tag that I've ever used that does not require being closed is the break tag, <b>&lt;br&gt;</b>, because all it does is add a line break. You'll sometimes see it formatted as <b>&lt;/br&gt;</b> instead of <b>&lt;br&gt;</b>, and that works as well. I'd recommend picking one and sticking to it.

Another thing to note is that tags can accept attributes that modify how it behaves, I'll give a few commonly used examples below as well.


On to the tags:


<b>&lt;a&gt;</b> is an anchor tag and used to hyperlink to other pages or to trigger a "send mail" event. Here are three common ways to use it

{% highlight html %}
<a href="http://www.example.com">This links to example.com</a>
{% endhighlight %}

The "href" attribute is where you direct the link to, always remember to add the "http://" or "https://" at the front of the link otherwise it will not work.

{% highlight html %}
<a href="http://www.example.com" target="_blank">This links to example.com, but in a new tab or window</a>
{% endhighlight %}

Here, the "target" attribute is what forces the link to open in a new window or tab. There are more values (that's the "_blank" part) that it accepts, but I've never had the need for them.

{% highlight html %}
<a href="mailto:email@example.com">This triggers a send mail dialog</a>
{% endhighlight %}

The "href" attribute accepts a few different kinds of values, and one of it is the "mailto" value. 



<b>&lt;p&gt;</b> is the paragraph tag. When you're writing in HTML, you can always manually hit "enter" a couple of times to create paragraphs, but it's not advisable because different situations might render it differently. Hell, sometimes it won't even be rendered at all so you'll end up with one big block of text instead of various paragraphs.

<b>&lt;h1&gt;</b>, <b>&lt;h2&gt;</b>, <b>&lt;h3&gt;</b>, <b>&lt;h4&gt;</b>, <b>&lt;h5&gt;</b> tags are header tags. HTML only supports up to five basic tags, though there are many ways you can tweak later on. These tags would be the subhead, lead_in etc of the NG world.

<b>&lt;i&gt;</b> is for italics, <b>&lt;b&gt;</b> is for bold, <b>&lt;s&gt;</b> is for strikethroughs.

<b>&lt;ul&gt;</b> is to create an unordered list, and once you open it, you'll need to fill it with <b>&lt;li&gt;</b> list items. At the end of it, you'll have to close it off as well. Another option is to use a numbered/ordered list with <b>&lt;ol&gt;</b>.

{% highlight html %}

<ul>
    <li>Kai</li>
    <li>Chris</li>
    <li>Caitlin</li>
    <li>Emily</li>
</ul>

{% endhighlight %}


will generate 

* Kai
* Chris
* Caitlin
* Emily

and

{% highlight html %}

<ol>Winners of the taco eating contest
    <li>Big Bob</li>
    <li>Hungry Harry</li>
    <li>Skinny Sam</li>
</ol>

{% endhighlight %}

will generate

* Winners of the taco eating contest
1. Big Bob
2. Hungry Harry
3. Skinny Sam


[w3schools]:    http://w3schools.com
