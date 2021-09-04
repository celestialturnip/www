---
title: "Lessons learned from releasing my first game"
date: 2021-09-03T15:44:57+09:00
draft: false
---

I made [FACEPONG](https://celestialturnip.itch.io/facepong) in 30 days as a way to start making and releasing games more consistently, inspired by [a327ex](https://www.a327ex.com/) and [Adam Pype](https://twitter.com/adampi). It's the first game I've ever finished making, after a dozen half-finished projects, so I wanted to share my thoughts and reflect on its development.

![FACEPONG gameplay](https://img.itch.zone/aW1nLzY4OTcxMTIuZ2lm/315x250%23c/FsChh%2B.gif#center")

## Some context
Until last summer, I had never done any game development.

I had been working as a software engineer for many years before I took a university course, [Practical Game Programming](https://www.athabascau.ca/syllabi/comp/comp369.html). As part of the course, I had built a few small-ish games for assignments using C/C++ with Allegro and I was hooked. 

For reference, software development has always been just "fine" for me. It's an easy way to earn money but it's not that exciting. Whereas when I built my first few games, I would spend hours just brainstorming ideas and trying to implement them. And so when the course ended, I wanted to continue making games.

But I didn't.

I would start a new project, prototype a new mechanic over the weekend, and within the next week or two, come up with a new idea and start over. I struggled to find an idea that I was both excited about and one that I thought I could execute well. I don't consider myself having much artistic ability and so when I would build these small little prototypes with free asset packs, I never felt I could turn it into a real game.

## What changed

After a year of a dozen half-finished projects, I decided that I wanted to become more serious about making games. I scaled down the number of hours I was committing to my regular full-time employment so that I could dedicate around 10-15 hours per week to game development.

I also decided to attempt to release a new game each month, based on what I saw two other developers doing. 

The first is [Adam Pype](https://twitter.com/adampi). He released [one game a month](https://papercookies.itch.io/) for 32 months (!!) before taking one of his monthly games and publishing it as a "big" game on Steam: [SPOOKWARE](https://store.steampowered.com/app/1574250/SPOOKWARE/). 

{{< tweet 1433200704097857538 >}}

The second is [a327ex](https://www.a327ex.com/) who was attempting to do [a game every 2 months](https://www.a327ex.com/posts/lessons_second_game/#a-game-every-2-months). As part of this, he released [SNKRX](https://store.steampowered.com/app/915310/SNKRX/) which has already sold 80k+ units and made over $200,000 revenue ([source](https://www.a327ex.com/posts/snkrx_log/#day-55-210709)).

As I continued to do more research on the idea of "regularly release small games", I found many other game developers and designers had a similar history of releasing many games before releasing at least one that I would consider successful:
- VVVVVV and Dicey Dungeons were Terry Cavanagh's 30th and 52nd [games](https://en.wikipedia.org/wiki/Terry_Cavanagh_(developer))
- Celeste was Noel Berry's [22nd game](http://noelberry.ca/) and its PICO-8 version was made in [four days](https://www.lexaloffle.com/bbs/?tid=2145)
- A Short Hike was Adam Robinson-Yu's [13th released game](https://adamgryu.itch.io/)

Another motivating example was Sokpop, a group of four game developers based in Utrecht, Netherlands. Each member of Sokpop would release one game every two months. As of March 2021, the four of them have collectively released [78 games][sokpop-interview]. Not to mention, their [Patreon](https://www.patreon.com/sokpop) is bringing in close to $6,000/month. With almost 2,000 supporters on Patreon, that means any game released under the Sokpop brand is guaranteed to have a pretty decent initial audience.

They were interviewed earlier this year and one part of the [interview](https://www.eurogamer.net/articles/2021-01-25-the-sokpop-collective-an-alternative-vision-of-game-development) resonated with me:

> Having only two months to make a game also means they cannot be precious about their ideas. They simply don't have time to chase a dream, and that, as strange as it sounds, can be an enormously liberating thing. Think how many developers lose themselves in over-ambitious ideas.

That said, I did see some other examples of game developers who just spent years working on a single game and were successful. For example, Eric Barone with Stardew Valley and Toby Fox with Undertale. However, in terms of my goals, I'm not trying to make millions of dollars with games. Right now, I just enjoy the game development process and want to try to improve my skills over the long term. I think it's also far less stressful since I can move on to a new project at the end of each month without feeling like I've invested a significant chunk of my life into the project.

[sokpop-interview]: https://www.eurogamer.net/articles/2021-01-25-the-sokpop-collective-an-alternative-vision-of-game-development

## How I got started

I came across [some advice](https://www.foddy.net/2018/06/flop/) by Bennett Foddy, developer and designer of QWOP, who wrote "it’s a worthwhile exercise for any game designer to make a chess variant, a dice variant and a Pong variant."

I looked through some old Atari games to see if there were any that I could revamp or remake. I saw Quadrapong (released by Atari in 1974) for the first time and thought there might be something interesting I could do with it. I first started just re-creating it in Godot and when I replaced the paddles with face sprites on a whim, I thought the game suddenly became more fun and challenging.

{{< tweet 1419079886380040192 >}}

I remembered some of Miziziziz's [advice](https://www.youtube.com/watch?v=5-iST0a69cI) on keeping a game to five levels and using public domain assets, so that's what I decided to do: a remake of Quadrapong with five levels using public domain assets.

## How I spent the month
Going into it, I didn't have a plan. I had a list of ideas for levels and fun gameplay elements, but with only 30 days to spare, I was very focused on just trying to get something working. Looking back, the general structure of the month ended up being:

- Week 1: build core gameplay structure (e.g. physics, player movement)
- Week 2: add five levels
- Week 3: fix bugs, add menus, polish
- Week 4: fix more bugs, add more polish, prepare marketing assets (e.g. create project page on Itch, record gameplay videos and make GIFs/screenshots)

The tricky thing is I did come up with the concept and basic prototype before I started the month officially. At that time, I only had my weekends for game development so I was still just trying out different ideas. But when I officially started my "30 days", I implemented everything from scratch. Going forward, I'm not sure how this will play out. I don't want to spend too long just trying to decide on an idea. But at the same time, I don't want to pursue an idea just because I feel I'm falling behind schedule. I'll have to see how the next project goes and re-evaluate from there.

I think the 50/50 split between "gameplay" and "bug fixing/polish/etc" makes sense. Especially when I see examples of Celeste for PICO-8 having been made in just four days, I think if you don't have a good gameplay loop within 1-2 weeks, I don't know if spending more time of the month will fix it. I think honing in on the gameplay loop as soon as you can is very important.

## Software engineering principles vs. yolo coding

No design document, no tests. Just simply coding and knocking things off my to-do list.

Part of the reason why I think regular software engineering is a bit boring is that there's so much planning-related work that needs to happen on many projects before you can start coding. You need to have meetings with different stakeholders (e.g. product manager, other teams, etc). You have to explain your plan and get approval from your manager/lead developers. And there are often decisions made outside of your control that you just have to live with (e.g. what programming language to use). I find most of the "high" from software engineering just comes from coding and solving technical challenges. I found I got this "high" more often when making FACEPONG than I probably ever have from regular software engineering work.

I did try to have an initial design document but... after spending a few minutes writing some things down, I started thinking: "Why am I wasting my time? This is a project that I'm only going to work on for 30 days. I already have a general idea of what the end product will look like." So I decided to close it and I have never opened it since. I think if I were to work on a game with two or three other people, it's important that there's a common understanding of what the game is and what it isn't. But as a solo indie dev working on small games, I'm not sure if there's much value.

With tests, I do enjoy writing tests (especially when I'm doing some significant refactoring). Having good code coverage with tests makes doing huge refactors easier, since you can instantly spot the problems and have some confidence that once all tests pass, that things should be close to done. Having no tests for FACEPONG made refactoring quite painful. I would try to change one thing, suddenly everything would be broken, and it would be unclear exactly how I should proceed. Furthermore, when I fixed a bug, it would have been nice to also write a test case to make sure it's been fixed.

Also, having no industry experience in game development, I'm not sure what testing/QA even looks like for larger-scale games. I know what it looks like for large-scale software (e.g. unit tests, integration tests, E2E tests, performance tests) but I'm not sure how to apply those techniques to a game engine like Godot. From my limited research, it's sparse and many tutorials I've watched on game development with Godot never mention the word "test".

## Marketing games

Ah, my least favourite subject.

I think marketing is super important - I just don't personally find it that fun to do since I don't get any of the "high" from completing tasks that I do with programming. Even for this project, I'm a little embarrassed by the result of it but I figured, I'll do some marketing tasks just so I can get used to the motions of doing marketing for a game. For example, setting up an Itch.io page with screenshots/GIFs, making a trailer on YouTube, and so forth.

I think for a real game that I would like to make some revenue off, marketing from day one is a good approach instead of just leaving it until the last day or week. I also think making games that are "easy to market" is also quite important. I would consider a game that's "easy to market" as one where within a few seconds of watching some gameplay, you instantly know what the core gameplay is and you want to try it.

When I think of games that did this well, holedown by [grapefrukt](https://twitter.com/grapefrukt) and Mixolumia by [davemakes](https://twitter.com/davemakes) come to mind:

{{< youtube id="WYME5YC2IbY" title="holedown launch trailer" >}}

{{< youtube id="AC8AAkjTSTc" title="mixolumia launch trailer" >}}

I also wonder once you've built a strong following of fans that either subscribe to your updates or pay you monthly on Patreon for example, if active marketing becomes less important. If you have 2,000 followers, there's probably some percentage that stream games on Twitch/YouTube which would most likely not be able to reach directly. a327ex also elaborates on this general idea of building followers in his [blog post](https://www.a327ex.com/posts/lessons_second_game/#steam-followers).

For now, I feel I'm still at a level where I don't have much confidence in what I produce so I don't want to waste people's time. For FACEPONG, I wanted to do a little bit of marketing just so I don't forget about it and I'm aware of things to keep in mind while I develop my game. Once I release a game I'm proud of, there are tons of different marketing channels I'll need to use (e.g. YouTube/Twitch streamers, YouTube channels promoting indie games, bloggers, etc).

## Daily devlogs and planning
Throughout the development of FACEPONG, I would start each day by updating my devlog with what I did the previous day. I decided to do devlogs because (a) I find them interesting/fun to read (b) perhaps they can be useful for marketing and (c) I thought it could keep me accountable.

I did not enjoy the approach I took with it. I found it a little bit of a chore, where I had to look at my commits for the previous day, and explain what I did. I think what I'll try to do next time around is focus my devlogs more on what I plan to do that day. That way, it'll help me organize my thoughts and I'll know exactly what I have to do that day.

I also like videos for devlogs, for example [Andrew Zi Zhen](https://www.youtube.com/watch?v=wxHE1laxKWg)'s and [DevDuck](https://www.youtube.com/watch?v=jzQWryIaL6c&t=86s)'s. I find they're the most fun to watch when they mix some personal life aspects into it. The ones I don't enjoy are just screencasts with some audio in the background. I find myself more drawn to the individual themselves and their personalities, so I think having a way to express yourself in a way that other people can relate to is very important. I won't do any for now but maybe in the future, I'll give it a try.

## Using my real name vs. anonymity 
I find myself struggling to decide if I should use my real name or not. I watched [Put Your Name on Your Game](https://www.youtube.com/watch?v=N4UFC0y1tY0) by Bennett Foddy and Zach Gage where they elaborated on many reasons why you should use a real name, instead of just a typical studio name (e.g. "XYZ Game Studio") and many of the reasons I agreed with.

What I eventually decided with is that for now, I'll release things under the alias "celestialturnip." Once I become more comfortable attaching my name to the things I release, then I think I'll slowly switch over. I struggled with this for quite a lot of time and made a list of game developers who use their real name vs. those that do not. What I generally found was:

- Many indie devs use an alias (even Eric Barone of Stardew Valley goes by ConcernedApe)
- Most indie devs with a small following are completely anonymous
- Most indie devs with at least one "successful" published game are not anonymous

For me, going with an alias was a way of getting around my fear of releasing games that I don't feel super confident about.

## Free games and pricing
FACEPONG is free. The next game I make will be free. I don't have any plans right now to charge people for games.

For me right now, building a community/following is far more important than making a few dollars on some games. By putting a price tag on my games, I would essentially limit my audience which there isn't any benefit to me.

I also wonder if some indie game devs charge too much for their games. I think what you want to avoid is having a game where someone regrets their purchase or feels it was good, but not worth it for the price. I see many games that are around the $7-$10 price range with not many reviews. I wonder if the game was just released at $3.99 for example, if this would have led to more natural word-of-mouth marketing (e.g. reviews and recommendations on Reddit).

## User testing
This is something I didn't do this time around but I'd like to incorporate somehow going forward.

Essentially, the only real user testing I did was getting my wife to play FACEPONG on a few occasions and (a) watching her play (b) listening to her feedback. It would be nice to have a small reliable group where I could share projects that are around 50-75% done so I can make some changes before releasing them. I'm not sure how other indie devs do this, especially when they're just starting. I see Discord being used quite frequently, but as someone who doesn't use it that often, it seems you need a few dozen people on it otherwise it seems kind of quiet.

## Conclusion && going forward
Overall, I'm happy with how this first month went. Even though it's not perfect, FACEPONG is definitely a five-level game that I think is somewhat fun. I also think with one under my belt, releasing games in the future will become easier the more often I do it.

For next month, I haven't decided what I'll work on. I might continue taking Bennett Foddy's advice and making either a dice or chess game - we shall see. :-)
