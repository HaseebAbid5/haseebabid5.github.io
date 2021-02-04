---
layout: post
title: Player Movement
subtitle: Uncover Complexities
tags: [Pokemon Clone, Technical, Programming, Movement]
comments: true
---

Far majority of games in existence have the player control a character/object's movement through some sort of input. There have been many examples of the different types of ways developers can have the user interact with their world, however the most common by far within 3D games are the third-person controller and the first-person controller. 

Most every mainline Pokemon game in the past has been a 2D game where the camera is positioned from a birds-eye view giving players a top-down mode of control. To translate that type of concept into 3D, I think its clear that a third-person approach is appropriate. This kind of style was sort-of implemented within Pokemon Sword and Shield but even then, aligning with the mediocre results of the games in general, the implementation is severely restricted.

![PokemonSSWalk](/assets/img/PokemonSSWalk.gif){: .mx-auto.d-block :}
<div align="center"><i>Pokemon S&S feature mostly fixed camera angles</i></div>

I will be using the same type of third-person camera, however it will be fully featured with rotating angles and such, exactly how most modern games do it.

![PokemonCloneCameraRotation](/assets/img/PokemonCloneCameraRotation.gif){: .mx-auto.d-block :}
<div align="center"><i>In-engine runtime camera rotation in my game</i></div>

## Third Person Controller

For the purposes of this project I will be using the  [Third Person Controller + Fly by Vinicius Marques Terra](https://homepages.dcc.ufmg.br/~allonman/). This package comes with the basics needed for controlling a character in third-person as well has a basic camera system. It also has a sort of mini state system, called "Behaviors", built into the script. The behaviors control the state context in which the character functions.

![PokemonCloneIdleWalk](/assets/img/PokemonCloneIdleWalk.gif){: .mx-auto.d-block :}
<div align="center"><i>From "Idle" behavior to "Walk" behavior</i></div>

This type of contextually driven state system makes it easier to manage when programming the player to utilize different mechanics within different behavioral context. For instance, notice how the movement of the player changes from normal to a strafing type of movement when the player is in the "Aim" state instead of the normal "Idle" or "Walk" state.

![PokemonCloneIdleWalkAim](/assets/img/PokemonCloneIdleWalkAim.gif){: .mx-auto.d-block :}
<div align="center"><i>From "Idle" behavior to "Walk" to "Aim"</i></div>

These different states allow for full customization of mechanics per state. The above gif is a good example of that and can be expanded upon to include crucial systems. For example, what would a Pokemon Clone be without Pokeballs?

![PokemonClonePokeballClone](/assets/img/PokemonClonePokeballThrow.gif){: .mx-auto.d-block :}
<div align="center"><i>A throw executed from the "Aim" behavior. Cannot be thrown from any other state.</i></div>

On top of all of those benefits is how easily compatible this system is with Unity's built-in animation state machine. Unity's animation state machine is used by calling the specified state with a variable change. These variables can be changed within the behavior system and allow the specified animation to be played accordingly.

![PokemonCloneAnimationStateMachine](/assets/img/PokemonCloneAnimationStateSystemgif.gif){: .mx-auto.d-block :}

That about covers the entirety of the player controlling system that I have used and built upon for this Pokemon clone. There will likely be more added to it. Something that I can think of right off the top of my head is having the player ride a bike or scooter, as is common in the actual Pokemon games. This will require me to create a new custom behavior in order to manage the movement of the bike/scooter along with the player accordingly. Stay tuned for more updates!