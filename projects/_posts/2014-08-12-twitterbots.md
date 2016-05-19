---
title: "Twitterbots"
subtitle: "Creating absurdity and subtle profundity"
layout: post
category: projects
tag: "Creative Programming"
permalink: /projects/twitterbots
---

A twitterbot is more-or-less an automated text generator that spews spam, poetry, or interacts with other twitter users. I built my twitterbots, <a href="http://twitter.com/writingassnbot" target="_blank" >@WritingAssnBot</a>  &  <a href="http://twitter.com/MakesTheHeart" target="_blank" >@MakesTheHeart</a>, using Python. <a href="http://twitter.com/alexanderussel1" target="_blank" >@alexanderussel1</a> is written in ruby with the help of some open-source code.
<br>
<br>

# Writing Assignment Bot

<a href="http://twitter.com/writingassnbot" target="_blank" >@WritingAssnBot</a> uses a mad-lib style algorithm to formulate writing assignments every hour on the hour. Give it a follow and you'll soon be knee deep with things to write about.

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Hammer-Out a metaphor defining New York, in 632 words or more.</p>&mdash; Writing Assignments (@WritingAssnBot) <a href="https://twitter.com/WritingAssnBot/status/729506200040013824">May 9, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
<br>

# Makes the Heart Grow Bot

<a href="http://twitter.com/MakesTheHeart" target="_blank" >@MakesTheHeart</a> pulls words from two gigantic word lists composed of nouns and adjectives which then complete {noun} makes the heart grow {adjective}. 

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr">attachment makes the heart grow annoying.</p>&mdash; Heart Grow (@MakesTheHeart) <a href="https://twitter.com/MakesTheHeart/status/523685061766701057">October 19, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
<br>

# Alexanderussell?

<a href="http://twitter.com/alexanderussel1" target="_blank" >@alexanderussel1</a> is an alter-ego bot based on open-source e-books code. The program reads <a target="_blank" href="http://twitter.com/alexanderussell">my tweets</a> and compiles them into a model that it then uses to create new tweets. There is a bit of logic that attempts to pair words in order to piece semi-coherent sentences together. 

<blockquote class="twitter-tweet" data-conversation="none" data-lang="en"><p lang="en" dir="ltr"><a href="https://twitter.com/AlexandeRussell">@AlexandeRussell</a> <a href="https://twitter.com/SBGilbreth">@SBGilbreth</a> I&#39;m not a solitary invention but a collaborative creation.</p>&mdash; Alexander Russell? (@alexanderussel1) <a href="https://twitter.com/alexanderussel1/status/728041176637554688">May 5, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

The same logic applies when tweeting at the bot, as it will try to respond with sentences containing words close to the words you've used when tweeting at it.

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr"><a href="https://twitter.com/AlexandeRussell">@AlexandeRussell</a> sound is energy moving through matter and a landscape</p>&mdash; Alexander Russell? (@alexanderussel1) <a href="https://twitter.com/alexanderussel1/status/723275046672723968">April 21, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

The rhetoric produced varies in intensity and borders between poetry, philosophy, semi-sentient ramblings, absolute absurdity, and occasionally, utterly dismal thoughts.

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">To condense fact from the thoughts, because it was not reality, because reality lay on the thighs of cuban women.</p>&mdash; Alexander Russell? (@alexanderussel1) <a href="https://twitter.com/alexanderussel1/status/723768619105136641">April 23, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
<br>

<br>

# Creating a home for the robots

<figure class="img-left">
<img style="max-width:300px;" src="/img/projects/raspberry-pi.jpg" />
</figure>

With the exception of the alter-ego bot, I set up my bots to live on a raspberry pi that sits under my TV. Raspberry pis are cheap, small, and use far less energy than a laptop or computer. Turning a pi as a server is a great way to house small applications that need to be constantly running and connected to the internet. Additionally, it only uses about 2.1 watts compared to the 11-80ish watts consumed by a Macbook Pro. I opted to run my pi "headless" (meaning no monitor/keyboard/mouse connection) and I can ssh into it to upload, edit, and run programs. 

<img src="/img/projects/raspberry-pi-ssh.png" />


<script>
$(window).on('load', function() {
    $('iframe[id^=twitter-widget-]').each(function () {
        var head = $(this).contents().find('head');
        if (head.length) {
            head.append('<style>.EmbeddedTweet { max-width: 100% !important; }</style>');
    }
        $('#twitter-widget-0').append($('<div class=timeline>'));
    })
});
</script>
