# Alternate 100-Sided-Die Advantage Mechanics For Tabletop Roleplaying Games (TTRPG)

The notebook in this repo looks at different ways to calculate advantage or disadvantage for roleplaying games, such as Mythras or Call Of Cthulhu, both of which use a similar 100-sided-die (d100) system. *Note for the uninitiated: In practice, a d100 is actually just two d10's, with one acting as the tens place and the other acting as the ones."

If you've played Dungeons & Dragons, you're likely familiar with the concept of "advantage." You roll two d20's and take the better option. "Disadvantage" does the opposite. These same mechanics can be applied to rolling two 2d100's.

The suggested, alternate method for advantage with d100's capitalizes on the fact that it's actually two dice. You roll the two d10's and try out both permutations, where the tens and ones are switched. For example, a roll of `4` and `7` could either be `74` or `47`, and the one you end up with depends on whether or not you've got disadvantage or advantage.

My friend who invented this mechanic wanted to see how this pans out numerically, so I ran a couple million simulations of dice throws and plotted the results in the attached notebook. We got some pretty cool, wobbly distributions. Go check em out!
