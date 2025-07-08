---
title: "Beat Heisters"
lang: en
page_id: beatheisters
date: 31/05/2021
project_type: game
header_image: /assets/images/projects/beat_heisters/beatHeistersFront.png
featured: false
vertical_card: false
tags:
  - Unity
  - Windows
---


<div class="quote-shadowbox">
Hold your ground after robbing a bank against the police, everything by the rhythm.
</div>
<!--content-->


<video style="display: block; margin: 0 auto;" width="75%" height="auto" controls>
  <source src="/assets/videos/projects/beat_heisters/beat_heisters_gameplay.mp4" type="video/mp4">
Sorry, video could not be loaded :(
</video>

During my Bachelor's Degree in Computer Engineering studies at University of Jaén, the "Multimedia Systems" subject served as an introduction to multimedia technologies for common codec used in image, video and audio file formats. As our final project, we made a 2 person group to build a rhythm game prototype.

<h2>Third person gameplay</h2>

<div class="flex_image_right">
  <div style="flex: 1 1 35%">
    <p>
      The game itself isn't complex, but includes some curious mechanics. The main objective is to hold your ground in a robbed bank, standing against the police using three different weapons:
    </p>
    <ul>
      <li><strong>Assault rifle</strong>: Your main weapon, shoots a bullet in every beat detected by the system.</li>
      <li><strong>Shield</strong>: Blocks incoming forwards shots, only active at the beat.</li>
      <li><strong>Grenade</strong>: Throws a grenade each beat with a considerable refresh time, but can defeat multiple enemies.</li>
    </ul>    
  </div>
  <div style="flex: 1 1 65%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/beat_heisters/beatHeistersStoreroom.png" />
  </div>
</div>


<h2>The interesting part: <i>onset</i> detection</h2>

Our efforts were focused on a system capable of beat detection for any sound track. These systems are a real challenge, given the massive amount of musical styles and each artist interpretation, but there's always some patterns common to them all.


<div class="flex_image_right">
  <div style="flex: 1 1 60%">
      <p>
        Any musical work follows a given rhythm as a repeated sound equally spaced during the track; this is what our systems detects to define when the game action occur. While the music plays, a background analysis is made over the signal frequency, building a curve over time peaking at most intense musical notes.
      </p>
  </div>
  <div style="flex: 1 1 40%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/beat_heisters/onsetCurve.png" />
  </div>
</div>

Using this curve, our implementation normalizes it with a local time window, isolating the curve peaks even more. After filtering and checking repeating patterns for those peaks, we achieve an approximated <i>tempo</i> for the current song.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/beat_heisters/onsetCurveNormalized.png" style="width: 60%; margin: auto;">
</div>
