So we had a pretty long conversation last night about fury prot vs deep prot. I wanted to bring some numbers to the conversation.

## First, some baselines:
 - Fury prot is a spec that relies on the natural threat that comes along with damage production, Deep prot will rely more on static threat that is inherent to certain abilities
 - I'm not going to count the healing threat from bloodthirst, it's small and I'm lazy. It is there though.
 - The DPS numbers do not count the ~300 damage (before mitigation) shield slam does
 - The specs may not be 100% right, but they're close enough for the DPS comparos
 - The gear used for DPS sim was identical
 - Heroic strikes are used, but we're not counting any static threat - In theory, fury prot casts significantly more heroic strikes as it's a good rage dump
 - Both specs cast sunder armor, but fury should end up with more casts as it has more rage avaliable
 
## Fury:
Fury prot has a number of things that generate threat, and it's mostly centered around doing more damage
 - Rage is generated in two basic ways : taking damage and dealing damage (white damage specifically)
 - Flurry - 30% increased attack speed for the next 3 swings after a critical strike. This helps both 1h and DW
 - Enrage - 25% damage for 12s or 12 swings, which ever ends first.  more damage output equals more rage generation, and more DPS output
 - Deathwish - a "boost my threat" button
 - Bloodthirst - straight damage with a small heal

### 1h
This is the warrior sim looking at DPS output for 1 handed (so with shield) DPS output in Beatus' normal tanking gear
DPS: 543
![1h Fury Prot](/images/1h_fury_prot.png)

### DW
This is the same warrior sim, same gear, except using dual wield.  Notice the stark increase of ~230 DPS or almost a 50% increase in damage output
DPS: 778
![DW Fury Prot](/images/2h_fury_prot.png)

## Deep Prot:
Deep Prot loses a lot of the damage output tools fury gives. In return, you get access to some limited, early in tree mitigation talents.  It's worth noting that while conventional wisdom tells us "Deep Prot" is considerably heavier mitigation, this is not entirely true.  There exist 4 talents for mitigation in the entire warrior tree, and 3 of them are in prot, the other is arms
 - Shield Specialization - a must have for both Deep and Fury prot. 5/5 Baby
 - Toughness - 2% increased armor from items up to 10%.  Fury prot utilizes 4/5.
 - Anticipation - 10 points in defense, roughly equivalent to the defense provided by Wrath Helm.  Provides 0.4% dodge, 0.4% parry, and 0.4% block for a total of 1.2% mitigation
 - Deflection - 1% parry per point, up to 5% parry chance.  This can be integrated into Fury-Prot builds, as Beatus has 2% parry integrated into his spec.
 
 Deep prot utilizes the ultra-rage efficent shield slam in it's rotation. Shield slam costs 20 rage.  This makes a seemingly intuitive level of sense for OTs, as they tend to be more rage starved than a MT, who rarely finds rage generation to be a problem (At least from my experience, Fury-Prot ones certainly don't.  Can't speak for Deep Prot, but lets assume they don't hurt for rage)
 - Shield Slam - 250 static threat (think of this like unmitigated damage) + "weapon damage" (342-358 damage base + shield block value)
   - Block value is the block number on gear + str * .5
   - 8/8 Wrath gives +27 block value, not counting str
   - So given values of 300 strength, 27 block value, we have 177 bonus damage
   - 250 static threat + 350 shield slam damage + 177 bonus damage = 777 threat generated (before taking into account crit chance, which if we're generous, affects Bloodthirst and shield slam equally).  Crits do not affect the 250 static threat, so it's just ("weapon damage" + block value + 0.5*STR)*2 in the case of a crit
   - Deep prot still utilizes all the rest of the bread-and-butter threat generating skills such as Revenge, Sunder armor, and Heroic strike.  

### 1h Deep Prot warrior sim (same gear as the fury sim above)
DPS: 312
![1h Deep Prot](/images/1h_deep_prot.png)

### DW Deep prot warrior sim (same gear as fury sim above)
DPS: 464
![DW Deep Prot](/images/2h_deep_prot.png)

As we can see from the sim, the amount of damage done by Deep prot is considerably lower.  THis surprises noone though, right?  We knew that.  The assumption we are running however is that with all this new threat being built into our deep prot ability (Shield slam, the only ability available soley to deep prot boiz), we rely less on the natural threat generation of damage output.  Now we have previously estabilished that with the exception of swapping shield slam for bloodthirst, the rotations for fury prot and deep prot are exactly the same.  The next logical question any discerning tank-to-be would ask is this: what's the difference in threat generation between a Bloodthirst and a Shield Slam? Buckle up boys, that's where we're going.

## Some real world bloodthirst damage numbers for ThreatDream and Beatus (This is mostly TL;DR'd at bottom, scroll through if you want): 

### ThreatDream

#### Vek (since that was the topic of conversation)

|sourceName|destName|"avg(amount)"|"max(amount)"|
| ------------------- | --------------------- | ----------- | -------- |
|"Threatdream-Netherwind"|"Emperor Vek'nilash"|"454.4710743801653"|1092|

#### All AQ mobs

|sourceName|destName|"avg(amount)"|"max(amount)"|
| ------------------- | --------------------- | ----------- | -------- |
|"Threatdream-Netherwind"|"Anubisath Defender"|"698.9230769230769"|1254|
|"Threatdream-Netherwind"|"Anubisath Sentinel"|"837.95"|1367|
|"Threatdream-Netherwind"|"Anubisath Warrior"|444|492|
|"Threatdream-Netherwind"|"Battleguard Sartura"|567|671|
|"Threatdream-Netherwind"|"Beatus-Netherwind"|288|288|
|"Threatdream-Netherwind"|"Emperor Vek'nilash"|"454.4710743801653"|1092|
|"Threatdream-Netherwind"|"Fankriss the Unyielding"|"795.5555555555555"|1256|
|"Threatdream-Netherwind"|"Lord Kri"|922|1356|
|"Threatdream-Netherwind"|"Obsidian Eradicator"|"862.4"|1319|
|"Threatdream-Netherwind"|"Princess Huhuran"|"737.2"|1461|
|"Threatdream-Netherwind"|"Princess Yauj"|"744.3333333333334"|1356|
|"Threatdream-Netherwind"|"Qiraji Brainwasher"|"971.5"|1465|
|"Threatdream-Netherwind"|"Qiraji Lasher"|"429.3333333333333"|522|
|"Threatdream-Netherwind"|"Qiraji Scarab"|"541.5"|693|
|"Threatdream-Netherwind"|"Qiraji Scorpion"|"361.3333333333333"|506|
|"Threatdream-Netherwind"|"Spawn of Fankriss"|457|457|
|"Threatdream-Netherwind"|"The Prophet Skeram"|"851.5"|1293|
|"Threatdream-Netherwind"|"Vekniss Borer"|485|485|
|"Threatdream-Netherwind"|"Vekniss Drone"|372|372|
|"Threatdream-Netherwind"|"Vekniss Guardian"|"821.3"|1368|
|"Threatdream-Netherwind"|"Vekniss Hive Crawler"|"780.8333333333334"|1354|
|"Threatdream-Netherwind"|"Vekniss Soldier"|"865.5"|1433|
|"Threatdream-Netherwind"|"Vekniss Stinger"|"617.5"|1179|
|"Threatdream-Netherwind"|"Vekniss Warrior"|536|536|
|"Threatdream-Netherwind"|"Vekniss Wasp"|"426.8333333333333"|522|
|"Threatdream-Netherwind"|Vem|"867.6"|1461|

### Beatus

#### Vek (since that was the topic of conversation)

|sourceName|destName|"avg(amount)"|"max(amount)"|
| ------------------- | --------------------- | ----------- | -------- |
|"Beatus-Netherwind"|"Emperor Vek'nilash"|"452.0103092783505"|1271|

#### All AQ mobs

|sourceName|destName|"avg(amount)"|"max(amount)"|
| ------------------- | --------------------- | ----------- | -------- |
|"Beatus-Netherwind"|"Anubisath Defender"|"668.6981132075472"|1242|
|"Beatus-Netherwind"|"Anubisath Sentinel"|"654.75"|1351|
|"Beatus-Netherwind"|"Anubisath Warrior"|731|1002|
|"Beatus-Netherwind"|"Battleguard Sartura"|"881.6153846153846"|1348|
|"Beatus-Netherwind"|"Emperor Vek'nilash"|"452.0103092783505"|1271|
|"Beatus-Netherwind"|"Fankriss the Unyielding"|"880.4444444444445"|1542|
|"Beatus-Netherwind"|"Obsidian Eradicator"|"910.3333333333334"|1266|
|"Beatus-Netherwind"|"Princess Huhuran"|"637.0625"|1156|
|"Beatus-Netherwind"|"Princess Yauj"|"971.4"|1960|
|"Beatus-Netherwind"|"Qiraji Brainwasher"|"732.6666666666666"|988|
|"Beatus-Netherwind"|"Qiraji Lasher"|"399.6666666666667"|478|
|"Beatus-Netherwind"|"Qiraji Scarab"|"380.42857142857144"|519|
|"Beatus-Netherwind"|"Qiraji Scorpion"|366|366|
|"Beatus-Netherwind"|"Sartura's Royal Guard"|431|431|
|"Beatus-Netherwind"|"The Prophet Skeram"|"1268.5"|1816|
|"Beatus-Netherwind"|"Vekniss Borer"|1130|1130|
|"Beatus-Netherwind"|"Vekniss Drone"|"444.6666666666667"|558|
|"Beatus-Netherwind"|"Vekniss Guardian"|"752.1052631578947"|1376|
|"Beatus-Netherwind"|"Vekniss Hatchling"|457|457|
|"Beatus-Netherwind"|"Vekniss Hive Crawler"|"658.1666666666666"|814|
|"Beatus-Netherwind"|"Vekniss Soldier"|"740.1666666666666"|920|
|"Beatus-Netherwind"|"Vekniss Stinger"|699|699|
|"Beatus-Netherwind"|"Vekniss Warrior"|1059|1459|
|"Beatus-Netherwind"|"Vekniss Wasp"|999|999|
|"Beatus-Netherwind"|Vem|"931.4"|1318|


Vek represents a worst-case scenario for Fury-Prot tanks.  We are being asked to wear all mitigation gear, at the expense of hit so that we are tankier than usual.  Still, I'm hitting 470 threat bloodthirsts (450 from damage value in the above table Plus the 20 threat for the self-heal).  This is indeed lower than the expected 777 threat from shield slam.  It's important to note the subtle difference in empirically derived bloodthirst data from our logs that represents damage done to the boss, so it takes into account mitigated damage from the bosses armor values.  the 777 threat is before boss mitigation, and because no one runs deep prot, we don't have that data to show what mitigated damage looks like.  But even so lets pretend none of it is mitigated (absurd, I know, but Deep Prot needs all the help it can get, as you'll see soon), it would appear that there is a 300 threat/ 6 second (the cooldown of both these abilites) advantage to shield slam, yielding 50 increased threat per second over bloodthirst.

Now lets scroll back up to the sim (don't worry, I'll wait).  We can see that in the same gear, a fury prot 1 hander is going to do 543 dps while a deep prot 1 hander is going to do 312 dps.  because threat output is based upon damage output TPS = 1.495(DPS), you can read this as 811.78 TPS vs 466.44 TPS.  Add in the 50 TPS increase for shield slam, and we have 811.78 vs 516.44 TPS, so Fury Prot is generating 295.34 TPS more in the SAME GEAR.  Shield slam is a more rage efficent source of threat yes, but already we are starting to see that the TPS is lagging behind. Why? Lets take inventory of the remaining variables that caused this to happen:

- Flurry uptime.  Flurry is a fury ability that allows 30% increased attack speed every time you're crit.  more attack speed means more attacks.  More attacks means:
         1. More opportunites to rage dump with heroic strike
         2. more white hits to generate rage, see point 1.
         3. more opportunites to get another crit, procc'ing another flurry
         4. more opportunites to get Unbridled Wrath, 40% chance on hit to generate 1 rage point.
- Enrage - this talent increases melee damage bonus by 25% for 12 hits or 12 seconds, whichever comes sooner after being crit.  this is hopefully pretty negated during Vek, because we are trying our hardest to push crits and crushes off the hit table using shield block, so we are under-utilizing Enrage on this particular encounter. But on other fights, this shits huge.  

In fairness to Deep Prot, I have neglected some positive varibles in the Deep prot tree as far as rage generation goes, and they are as follows:
1. While both shield slam and bloodthirst are on a 6 second cooldown, shield slam does utilize 10 less rage every 6 seconds, meaning you have 2.5 rage per second more to spend on other abilities.
2. Anger Management - this talent adds 1 rage every 3 seconds (0.33, repeating of course, rage per second)
This means that Deep prot afford an additional 2.83 rage per second to use on abilities.  However, don't forget that Deep Prot is 181 TPS in the hole right now.  I cannot think of a single way you could make up for 181 TPS with 2.83 rage per second (but I'd encourage someone to try).  

Essentially, Fights like Twin Emps represent the epitome of when a Deep Prot tank is useful.  When the tanks aren't able to utilize threat-gen gear for fear of going splat, it makes an intuitive level of sense that being efficent is king.  This math shows, that even while being more efficent, and having as close to a "home field advantage" as this build is gonna have throughout our current level of content, *Fury Prot still puts out better TPS numbers than Deep Prot*


So we talked about threat production, used real world examples that actually favor Deep Prot, and came to a conclusion, putting to bed the notion that Deep Prot outperforms Fury Prot from a threat standpoint.  Next point to cover is Mitigation.  

Deep Prot: +5% shield block chance                                  Fury Prot: +5% shield block chance
           +10% armor contribution from items                                  +8% armor contribution from items (me)  +6% (beatus)
           +5% Parry chance                                                    +2% Parry chance (beatus) +0% (me, because I'm an asshole who takes piercing howl)
           + 10 defense skill (0.4% dodge, 0.4% parry, 0.4% block
           
As we can see here, there are some slight advantages from a mitgation standpoint to being Deep Prot.  
 - 2-4% armor contribution from items
 - 3-5% increased parry chance
 - 1.2% mitigation chance from the defense skill.  
 That is significant in some situations, without a doubt.  However, when you compare these bonuses to the dodge, parry, block you get from itemization, it seems to be a much smaller piece of the puzzle, in my mind at least.  5 talent points in Anticipation is worth less than the +defense skill on Wrath Helm alone.  3 talent points is worth less than 1 ZG enchant.
 
 Finally, I want to talk about enconomy of itemization, and by that I mean how do we get as much bang for our buck as possible when choosing priority stats.  As we've proved above, if we want to increase the threat output from our shield slams, we need to get more shield block value and we need more strength.  Even for our fury boys, strength is important - it increases raw damage output.  It however has very little defensive utility.  
 
 Agility on the other hand, is king for fury prot warriors.  Agility is the main driver of crit chance, which as we learned above, drives flurry, which is one of the main drivers of Fury Prot DPS/TPS output.  20 Agi = 1% crit.  20 agi also becomes 1% dodge, making it an exeptional mitigation stat.  a 1% dodge means a 1% chance to take absolutely no damage from a mob, making it vastly superior to block, and a little worse than parry, because in theory, a parry will reset your attack timer, allowing you to hit the mob again sooner.  A block will push a crit or a crush off the hit table, but you still end up taking (mobs attack damage - your shield block value modulated by items).
 
 ## *TL;DR - For those who just want the cliffs notes, not the entire deep dive*
 
 ## Threat Output
 - Even with the best circumstances (tested above on Twin Emps, the most friendly Deep Prot fight yet), Deep Prot fails to generate as much threat as Fury Prot.  
 - This even includes the rage efficency talents that make Deep Prot seem more intuitively viable, but amount to only 2.83 rage per second
 - Fury Prot has room to continue to improve with itemization, while Deep Prot is reletively static in TPS output unless you're stacking STR like a madman, which means ignoring other great mitigation stats
 - Fury Prot TPS output is more a function of DPS, meaning when Fury Prot tanks are DPSing, they are DPSing harder than than Deep Prot, making them more useful for single mob encounters, and tightening kill times.  
 
 ## Mitigation
 - Deep Prot and Fury prot share a lot of the same mitigation talents.  There's Mitigation talents inherent to both builds, but Deep prot does have more
 - Overall, Deep Prot can be expected to take advantage of 10 Defense points, 3-5% Parry depending on talent build, and 2-4% armor contribution from items
 - In both cases, the grand majority of mitigation comes from itemization and gear loadouts combined with consumables, which are available to both specs
 - There may be a benefit to the healers for having this extra mitigation, but it may not be outweighed by the faster kill times from having higher DPS tanks (though this is just bullshitting, and has no concrete evidence either way)
 
 ## Flexibility
 - Fury Prot makes a much better DPS OT spec.  They do soooo much more damage than deep prot (see above)
 - Deep Prot can stance dance, making it much easier to charge and be more mobile.  Some might argue this is exactly what a bear tank is for, but it's a clear benefit nonetheless.
 - Fury Prot is limited to having to save bloodrage to cast Intercept.  
 
### I hope this deep dive was useful to someone.  If anything, it allowed Beatus and I to add numbers and concrete evidence to what we feel we have already empirically determined is truth.  I forsee the overall benefits of Fury Prot spec for all Warrior tanks outweighing the benefits of Deep Prot at this time, and likely moving forward as well.  Threat problems only get worse with Deep Prot as content progresses, while the mitigation benefits don't really WoW me.  
 
 

