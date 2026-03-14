<div align="center">
  <h1>¸,ø¤°`°¤ø,¸¸,ø¤°`°¤ø,¸  OrbiPi  ¸,ø¤°`°¤ø,¸¸,ø¤°`°¤ø,¸</h1>
</div>

## A Pi-Based Orbital Simulator

A 2D orbital mechanics simulator with a twist: it demonstrates how changing the value of Pi would affect satellite navigation and orbital stability.

<img width="1800" height="860" alt="SCREENSHOT_1800x860" src="https://github.com/user-attachments/assets/7dd958b1-1dc3-4623-9514-365d04394e8b" />

<br><br>

If the correct value of Pi is used, the "navigation system" will calculate the correct thrust to keep the satellite in orbit. If an incorrect value of Pi is entered, the satellite's navigation system will incorrectly adjust its speed, causing the orbit to decay (crashing into Earth) or become eccentric (flying off into space).

Time is compressed, so you only need a few seconds to observe the effect of an incorrect Pi entry, instead of hours.

It's very fun to play with new, assumed values of Pi and observe what happens.

The live version can be found here: https://cabecao.net/OrbiPi

Started writing it in GDScript for the game engine Godot 4.6.1; however, the Web Export proved too bloated, slow to load, and poorly performing. Don't get me wrong, I love Godot, but today its Web Export template is lacking, so I ported it to HTML/CSS/JavaScript. For this, as an exercise, I opted for a 100% AI generated code, no manual fixes, tweaks, etc, just prompts; Oh boy, it was a painful experience, at least in this specific use case, but that's another subject.

The script uses the Velocity Verlet symplectic integrator for its simulation (which I don't fully master), considered highly stable.

The source code can be found under the **src** folder; it's mostly a fully self-contained code, with only the earth image and the favicon as external files.


Makes use of: https://commons.wikimedia.org/wiki/File:Earth_icon_2.png \
LinkedIn article: https://www.linkedin.com/pulse/happy-pi-day-2026-pi-based-2d-orbital-mechanics-cristiano-monteiro-qjydf
