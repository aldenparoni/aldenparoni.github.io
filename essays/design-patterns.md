---
layout: essay
type: essay
title: "A Smashing approach of design patterns"
date: 2023-04-27
published: false
labels:
- Design Patterns
---

<div class="text-center">
    <img class="py-4" src="../img/smash-wallpaper.jpg" width="1296px" alt="Super Smash Bros. Ultimate wallpaper of all characters">
</div>

One of my favorite games from my childhood that I still play to this day is _Super Smash Bros._ It's a party fighting game for Nintendo consoles where you play as iconic characters throughout video game history and try to knock your opponent(s) out of the screen. As a kid I used to play _Super Smash Bros. Melee_ on the GameCube. I wasn't any good at the game -- my 4-year-old pea brain had no idea what I was doing -- but I'd still have a blast playing. It was when I entered high school that I seriously wanted to get better at Smash. There was an esports club at school that specialized in Project M, a modded version of _Super Smash Bros. Brawl_ on the Wii which made gameplay feel similar to _Melee_. It had been a long time since I played Smash, but in that time I had grown interest in entering the competitive scene in some capacity. I figured joining the esports club was my way in.

## _Super Smash Bros._ but it's an analogy for design patterns

Before I continue, I feel obliged to explain a bit more about how a kids game could spawn such a massive and dedicated competitive scene that continues to grow till this day. When played at the highest level, Smash is a fast-paced and highly complex fighting game. With traditional fighting games like _Street Fighter_ and _Tekken_, you have to attack your opponent until they run out of health, and the best way to do that is by performing attack combinations, or combos. Normally these combos can only be executed by pressing a specific sequence of buttons on your controller. The beauty of Smash is that combos can be created on the fly by the player, and the level of difficulty in executing these often-improvised combos is through the roof. It's for that reason that clips like the legendary [wombo combo](https://www.youtube.com/watch?v=pD_imYhNoQ4) include such explicitly strong and exciting reactions. In addition, despite the simple controls, the finer details are what gives Smash its complexity. Matches can be won by the margin of a single pixel or frame. Split-second decisions are made all throughout the match, hence you need to be on your toes when you have the controller in hand.

<img align="right" src="https://ggn00b.com/wp-content/uploads/2020/09/waveland-1.gif" width="300px" alt="wavedashing gif">

Now I digress. The first couple of weeks in the esports club consisted of many losses. These losses were rarely ever close affairs. I'm pretty sure I was the worst player in the club at that time. I was losing to everyone left and right. I knew the fundamentals, but it's hard to apply them when being juggled in the air with nothing else to do but to accept defeat. Whenever I was not getting hit, I would just throw literally any move at my opponent hoping something would land, until I leave myself open for another merciless combo. Needless to say, some coaching would definitely get my head out of the water. Thankfully one of the best players in the club, Tyler, spared some time to teach me about a bad habit that most people in the club had that could easily be capitalized on.

In this coaching session with Tyler, one move that most of my opponents would do as they are falling back down to the ground is throw out literally any move. Aggressive, but reckless. In Melee and Project M, there's a movement technique called a wavedash, wherein you make yourself slide a short distance on the ground. It's different from running and then stopping, because the small timespan between being in the middle of stopping and actually stopping leaves you vulnerable for attacks. Wavedashing eliminates that vulnerability, allowing you to throw out a move immediately after performing a wavedash. Tyler told me this: when your opponent threatens to throw out an attack, dodge by wavedashing away, and then punish with a strong attack of your own.

## Applying the mindset to programming

One could say that the wavedash is a Smash design pattern. When I actually applied the wavedash into my matches, it produced amazing results. I finally started winning matches. It solved the most common problem that I ran into during my losing streak. As I continued using the wavedash, I found that I could use it offensively as well as defensively. I can use it to adjust my position in relation to where my opponent is to prepare for my next move. I used to finish last in tournaments; at my highest, I finished in 3rd within the club. The important thing about the wavedash, along with other advanced movement techniques in Melee, is not simply knowing how to do it, but actually using it to position yourself for success.

As I continue my portion of the work for the Ohana Scholars application project, I realize that I had been using design patterns the entire time. One of the issues I ran into was to figure out a way to make distinctly clear on the home page that the user was logged in. The idea I thought up was a simple message on the home page that said, "Hello, (user's first name)!" I used the observer design pattern to solve this issue by subscribing to the Student collection so I could take the data from the user's Student object to actually address them as their first name.