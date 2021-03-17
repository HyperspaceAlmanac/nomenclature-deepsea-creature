# Psychic Cyborg Battlers

# Overview
This is a C# command line console multiplayer turn based strategy game.
Everything will be text based, but interactive with screen refresh on key presses.
Two players will use the same keyboard to play at the same time.

I want to experiment with making a fun strategy game with only the very basic display.
It is going to use a turn based system that I have thought of years ago but keep on
running into obstacles in implementing it. This time I want to commit to it and see it through.

# Educational Purposes
I will be making this game to practice C#, some programming concepts such as interfaces,
and to show that I can write clean and efficient code.

# Gameplay
Game will generate some randomized fighters for players to make teams from.
Players will the use the teams to fight.
In a way I want to make an interesting gatcha style game but multiplayer and
without gatcha.

# Turn Order Mechanics
Made a big breakthrough last night.

Each turn is broken up into multiple parts with both players choosing a formation,
attacking once and defending once.

Currently planning 6 character parties so that players have to choose 2 to attack with, and 2 from
remaining 4 to defend with.

In general, player attacking should be the one to pick actions last.
Might need to change the turn order a bit more.

Order will be (for P2 defending):
P2 formation (secret)

-> P1 formation (reveal both), P1 Choose Two (secret, for action 1)

-> P2 Choose Two (reveal both, for action 1), P2 choose defending action (scret)

-> P1 Choose attacking action(reveal both) -> Resolve

Switch Attacker and Defender

P2 Choose Two (secret, for action 2)

-> P1 Choose Two (reveal both, for action 2) -> P1 choose defending action (secret)

-> P2 chosoe attacking action (reveal both) -> Resolve

Then it goes to P1 defending, with P1 choosing Formation first.





