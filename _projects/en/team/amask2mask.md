---
title: "A Mask 2 Mask"
lang: en
page_id: am2m
date: 1/02/2026
project_type: game
header_image: /assets/images/projects/am2m/am2mFront.png
featured: true
vertical_card: false
tags:
  - Godot
  - Web
---

<div class="quote-shadowbox">
Hide in crowds and slip through security while collecting new masks for additional concealment options. Try it here: ><a href="https://imjustjc.itch.io/a-mask-2-mask"><i class="fa-brands fa-itch-io"></i></a><
</div>
<!--content-->

<h2>Game Jam theme and our idea</h2>

**A Mask 2 Mask** was our entry to the first [JaénJam](https://itch.io/jam/jaenjam-1), with the proposed theme being *Mask*. Right from the start, I got a clear idea to take advantage of the dual meaning of the word mask, for both the face accessory and as a synonym for concealing, going back to, as the main reference, the original Assassin's Creed entries where crowd stealth was part of the core gameplay mechanics.

Considering the limited time (JaénJam I spanned just for a weekend) and the need for quick development and playtesting, we chose the Godot engine as our main tool, using a top-down view and pixel art so we could focus on delivering an easy game to understand just from a quick look.

<h2>Gameplay mechanics</h2>

Upon stabilizing the idea, I took all the gameplay implementation in Godot tasks, leaving all the visuals to my teammate. First, playable character movement and item collecting were pretty much straightforward to get done, made as the foundation for the core mechanics: stealth and detection.

Detection itself was also solved easily with some rays and shapes casts, simply checking when a security guard has a line of sight from you, but concealing using the masks was the greater challenge. Over the levels, groups of NPCs wearing masks allow you to hide when selecting the same mask, so a basic inventory management was required.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/am2m/am2mLv1.png" style="width: 48.5%; margin: auto;">
  <img src="/assets/images/projects/am2m/am2mLv2.png" style="width: 48.5%; margin: auto;">
</div>

Upon solving these core mechanics, my last part was designing a few short levels for everyone to play, but time was not on my side as I only had a few hours left before submission. Although I tried to add three different levels, only two made the cut, but those ended up being nice, with a proper duration to keep people playing the game for a bit. Here, let me show you how both levels were drafted by hand:

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/am2m/am2mDraft.jpg" style="width: 30%; margin: auto;">
</div>

<h2>The Game Jam event</h2>

After taking part in a few gamejams, those a tough, but extremely rewarding events. Getting to know cool people and how they build their ideas in just a few days is clearly the best of a gamejam, more so when it is nicely managed by a great team (and they even gave us some themed goodies and snacks!). We all even got featured and interviewed about the event and our games! Check the videos (spanish audio only):

 - <a href="https://www.youtube.com/watch?v=GvwY-wL3-Kw">Mesón Sol <i class="fa-brands fa-youtube"></i></a>
 - <a href="https://www.youtube.com/watch?v=GofPoCvktsc">A Link to the Podcast <i class="fa-brands fa-youtube"></i></a>
