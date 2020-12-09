# Alternate 100-Sided-Die Advantage Mechanics For Tabletop Roleplaying Games (TTRPG)

## Game Mechanic Context

The notebook in this repo looks at different ways to calculate advantage or disadvantage for roleplaying games, such as **Mythras** or **Call Of Cthulhu,** both of which use a similar **100-sided-die** (d100) system. *Note for the uninitiated: In practice, a d100 is actually just two d10's, with one acting as the tens place and the other acting as the ones."*

If you've played **Dungeons & Dragons,** you're likely familiar with the concept of "advantage." You roll two **20-sided-dice** (d20) and take the better option. "Disadvantage" does the opposite. These same mechanics can be applied to rolling two d100's.

**Herein, the suggested, alternate method for advantage with d100's capitalizes on the *fact that it's actually two dice.*** You roll the two d10's and try out both permutations, where the tens and ones are switched. For example, a roll of `4` and `7` could either be `74` or `47`, and the one you end up with depends on whether or not you've got disadvantage or advantage.

## Visualizing 2d10 As A (Dis)advantaged 100-Sided-Die

My good friend Anthony, who invented this mechanic (and after whom I have been calling it "Rolling Tony"), wanted to see how this pans out numerically. I ran some code to simulate dice throws and plotted the results in the attached notebook. We got some pretty cool, wobbly distributions. Here is what I cosider the crown jewel of the lot, where rolling 2d10 with this new type of disadvantage is plotted in green, and the inverse in yellow:

![2d100 Tony](/images/2d10_tony_double.JPG)

These plots produce interesting behavior, namely in the amount that they fluctuate up and down. This is due to the fact that certain numbers in the 1-99 range **become impossible to roll under either condition.** For instance, a `91` is an *impossible output* when "Rolling Tony" with *disdvantage:* If you roll a `9` and a `1` on your 2d10, you must *always* take the `19`. The pattern maintains that the larger number always finds itself in the ones place. And thus, the higher the number, the less likely we are to achieve it. In the range of 90-99, the *only possible output* is `99`, since that is the only case where neither value can be larger than the other. The inverse is true of *advantaged* cases.

## Applying These Rules To 2d6

This line of inquiry was also applied to rolling 2d6 (two 6-sided-dice). A similar distribution was made, with more aggressive spiking due to the fact that **certain numbers in the 11-66 range cannot be rolled at all, in either situation:**

![2d6 Tony](/images/2d6_tony_double.JPG)

For instance, the numbers 11-20 (inclusive) can **never** be rolled, because the dice in question lack a 7, 8, 9, and 0 on their faces. Beyond these interesting "potholes" in the spectrum of possible outputs, the same logic as above holds.

## Use Cases

For the unitiated, the main use case of *any* advantage mechanic is to indicate a level of ease or difficulty with which something is being done in-game. If, for example, a player is trying to sneak up on a slumbering monster to steal its treasure, they then would have **advantage.** If however, the same beast was awake and angry, they would instead have to roll with **disadvantage** if they still attempted stealth. This use case, clearly, still work sin the new system by again assigning (dis)advantage.

Another place this mechanical suggestion *shines* is in the **"culture"** of it, per se. There is something (un)satisfying about rolling two dice, having to construct a best or worst case scenario from them, and then presenting the new concatenated number to your fellow players. It also makes for **heightened awareness of tension.** If, for example, the game master says you need an `80` to pass a skill check, but you have disadvantage on 2d10, you know that (based on mechanical possibility) there are *only three* numbers that can save you: `88`, `89,` and `99`. What once was a 20% success rate, has been slashed to 3%. The specific awareness of overwhelming odds makes any triumph even more satisfying. A plot illustrating this is as follows:

![2d10 w Success Threshholds](/images/2d10_tony_success.JPG)

And lastly, it's just fun! It's another way to make those clunky plastic number-bricks entertaining to toss at the table. I hope you use this system, and if you do please [tweet at me](https://twitter.com/zych_steven) or contact me on GitHub. Happy gaming!