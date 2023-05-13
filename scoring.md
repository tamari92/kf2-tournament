![alt_text](https://i.imgur.com/3TKZOVr.png)

# Tournament Scoring System
The Scoring System used in this tournament assigns teams **Points** based on their overall performance in the match.

There are three major components of the Scoring System:
- [Completion Score](#completion-score)
- [Score Bonus](#score-bonus)
- [Score Penalty](#score-penalty)


## Completion Score
**Completion Score** (CS) represents how far the team has made it through the game and is the backbone of the total score earned for the match.

Teams earn **1 Point** for every **1%** of a wave completed. This implies that completing an entire wave awards **100 Points** in total.

This further implies the following **maximum** CS values for each individual Game Length:
```
Short (4 Waves):   400 Points
Medium (7 Waves):  700 Points
Long (10 Waves):   1000 Points
```
**Partial credit** is awarded if the squad is wiped out before the wave ends.
In this scenario, Points are awarded based on how far the team made it through the wave before dying.

For example, if Waves 1 through 4 were fully completed, with the team wiping on Wave 5 at **141/253 ZEDs remaining**, then the team earns **400 Points** (for Waves 1-4), with the points earned for Wave 5 being calculated as:
```
CompletionScore = ((TotalZedsInWave - ZedsRemaining) / TotalZedsInWave) x 100 x PointsPerPercent
= ((253 - 141) / 253) x 100 x 1
= (112 / 253) x 100 x 1
= 0.5573 x 100 x 1
= 55.73
= 55 Points
```
**All fractional/decimal portions of the value are dropped**, which is equivalent to rounding down to the **nearest whole value**. The final value after this calculation then represents the team’s CS for that wave.

Thus, the team’s total CS for Waves 1-5 would be `400 + 55 = 455 Points`.


## Score Bonus
**Score Bonuses** are modifiers that **add** Points to the team's total score.

They are attributed from several sources and are focused on rewarding teams for playing well under specific conditions. Bonus points make up the bulk of the total score earned for a match and are what allow one team to pull ahead of another.

There are four Score Bonus categories:
- [Health Bonus](#health-bonus)
- [Time Bonus](#time-bonus)
- [Objective Bonus](#objective-bonus)
- [No-Medic Bonus](#no-medic-bonus)

**Score Bonuses are only obtainable by completing the match with a VICTORY**. In other words, **the Boss must be killed to secure the Bonus Points.** A full team wipe will result in loss of all Bonus points, leaving only the CS to be factored into the total score.

### Health Bonus
**Health Bonus** (HB) represents how *healthy* the squad is. It is a pool of bonus points that starts off at a large value and bleeds off as members of the team die.

The default HB for matches in this tournament is **600 Points.** Each time a squad member dies, the team loses **100 Points** from their HB pool.

This implies that the team can suffer up to **6 deaths total** before exhausting all of their Health Bonus.

HB is calculated *independently* of how many times each individual squad member has actually died. This means that the HB will be fully exhausted whenever the team suffers six *total* deaths, regardless of who has died thus far.

### Time Bonus
**Time Bonus** (TB) represents how *efficient* the squad is. It is a pool of bonus points earned by completing the match as quickly as possible.

Each map has its own associated Time Bonus value. When the match begins, the value of the Time Bonus begins to decease by a standard rate each second, with the rate increasing as the match continues.

The intervals at which the Time Bonus decay increases is dependent on the map in question, however the amount that the decay increases to is always the same for all maps played:

- **1 Point / sec** at the start of the match
- **2 Points / sec** when X% of the Time Bonus is remaining (dependent on map)
- **3 Points / sec** when Y% of the Time Bonus is remaining (dependent on map)

A very important consideration is that the **Time Bonus does not stop decreasing, even during the Trader period!**

On the other hand, the decay rate is affected directly by the speed of the game, meaning that **ZED Time** causes it to slow down to 20% of its rate.

In general, it is in every team’s best interest to optimize their Trader path, buy strategy, and overall positioning to maximize their efficiency during the Trader period (and thereby maximize their TB).
Utilizing the **SKIP TRADER** functionality is highly encouraged to save even more time and is pivotal for teams looking to maximize this bonus. Maximizing ZED Time Extensions is also essential for achieving a high Time Bonus score.

When the match is completed (boss killed), the team is instantly awarded the remaining value of the Time Bonus toward their total score for the match.

### Objective Bonus
**Objective Bonus** (OB) represents Map Objective completion.

Most maps have several Dosh Hold Zones (aka “Stand Your Ground”) that can be completed for bonus XP, Vault Dosh, and Dosh. Other maps have additional contextual objectives that can appear on specific waves (e.g. KF-Airship).

Completing any of these objectives awards **150 Points** toward the team’s OB.

It is important to note that for ALL objectives, the objective must be completed **in its entirety** for the team to be awarded Points. This means that for DHZs, the meter must reach 100%. For all other map objectives, the meter must read COMPLETE or 100%.

For a given map, Dosh Hold Zones will appear at a static location on each wave they are offered. This does not necessarily mean that they will always appear at the same location for all waves, but rather that they will always appear at the same location on that wave in particular. Furthermore, DHZs will appear on the same waves for each run of an individual map to keep things fair for all teams.

### No-Medic Bonus
**No-Medic Bonus** (NMB) is a special bonus that is granted for runs that are completed *without* a Field Medic.

Unlike the previous bonuses, NMB acts as a **multiplier to the total score** of the match. Specifically, NMB multiplies the Total Score by a factor of **1.50x (150%).**

This multiplier is applied *AFTER* all previous bonuses are added to and all penalties subtracted from the current score.

NMB exists to reward teams that manage to overcome the innate difficulty increase brought on by not having a dedicated healer present on the team.

In the event that a player should switch to or spawn into the game as a Field Medic, the bonus is immediately marked as **Void** and a message is printed to the chat box.

**It is NOT possible to revert this state once obtained.**

As an example, consider the following Completion Score (CS), Health Bonus (HB), Time Bonus (TB), and Objective Bonus (OB) values:
```
CS: 1000
HB: 200
TB: 1275
OB: 150
```
The calculation of the Total Score as a result of the NMB would go as follows:
```
TotalScore = (CS + HB + TB + OB) x NMB
= (1000 + 200 + 1275 + 150) x 1.50
= 2625 x 1.50
= 3937.5 Points
= 3937 Points
```

Similarly to the Completion Score calculation, **all fractional/decimal portions of the value are dropped**, which is equivalent to rounding down to the **nearest whole value.** The final value after this calculation then represents the team’s total score for the match.

Thus, the team would earn **3862 Points** in total for the match. Should the NMB be voided, the team would only earn **2575 Points** instead.


## Score Penalty
**Score Penalties** are modifiers that **subtract** Points from the team’s total score.

If the **No-Medic Bonus** is obtained, the score penalties are subtracted from the team’s total score **BEFORE** the NMB multiplier goes into effect. This results in a sharper decrease of Points overall compared to subtracting the penalty after the multiplier.

Currently, the only score penalty in use is the **Time Penalty** (TP). TP is acquired in the event that teams take *too long* to finish the match.

The actual value of the penalty is based off of the **PENALTY Time** value, a predetermined value that represents the maximum time it should take teams to beat the map under normal circumstances.

Teams lose **2 Points** for **every second** they take to complete the match after surpassing the PENALTY Time.

As an example, consider the following CS, HB, TB, and OB values:
```
CS: 1000
HB: 200
TB: 1275
OB: 150
```
Using the above values, the team’s total score before the penalty would be:
```
TotalScore = CS + HB + TB + OB
= 1000 + 200 + 1275 + 150
= 2625 Points
```
.. but now suppose the **PENALTY Time** is **1:00:00** (3600 seconds) and the team has completed the match with a time of **1:05:47** (3947 seconds).

This would result in a TP of:
```
TimePenalty = (CompletionTime - PenaltyTime) x PointLossPerSecond
= (3937 - 3600) x 2
= 337 x 2
= 674 Points
```
This value would then be subtracted directly from the total score, resulting in the team earning:
```
TotalScore = (CS + HB + TB + OB - TP)
= 2625 - 694
= 1931 Points
```
..or alternatively if the team had obtained the No-Medic Bonus:
```
TotalScore = (CS + HB + TB + OB - TP) x NMB
= (2625 - 694) x 1.50
= 1931 x 1.50
= 2896.5
= 2896 Points
```
As a result of the TP, the team would only earn **1931 Points** (2896 w/ NMB). This is a drastic decrease from the original value of **2625 Points** (3937 w/ NMB).

Though this decrease might seem harsh, it is tuned as such to strongly discourage strategies in which teams purposely draw out the length of the game in order to preserve Bonus, as this would generally be unfair to the other teams that took a normal amount of time to complete the match. Longer games also take longer to stream, and so this penalty exists for the convenience of the streamers, commentators, and spectators/viewers as well.

As teams begin to approach the penalty, a warning will be printed to the in-game chat box to warn players when they are within:
- 10 Minutes
- 5 Minutes
- 2 Minutes
- 1 Minute

.. from the penalty time.
