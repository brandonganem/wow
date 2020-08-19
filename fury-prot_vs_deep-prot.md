So we had a pretty long conversation last night about fury prot vs deep prot. I wanted to bring some numbers to the conversation.

## First, some baselines:
 - I'm not going to count the healing threat from bloodthirst, it's small and I'm lazy. It is there though.
 - The DPS numbers do not count the ~300 damage (before mitigation) shield slam does
 - The specs may not be 100% right, but they're close enough for the DPS comparos
 - The gear used for DPS sim was identical
 - Heroic strikes are used, but we're not counting any static threat - In theory, fury prot casts significantly more heroic strikes as it's a good rage dump
 - Both specs cast sunder armor, but fury should end up with more casts as it has more rage avaliable
 
## Fury:
Fury prot has a number of things that generate threat.
 - Flurry - 30% AS for the next 3 swings. This helps both 1h and DW
 - Enrage - 25% damage for 12s or 12 swings, which ever ends first
 - Deathwish - a "boost my threat" button
 - Bloodthirst - straigh damage with a small heal

### 1h
DPS: 543
![1h Fury Prot](/images/1h_fury_prot.png)

### DW
DPS: 778
![DW Fury Prot](/images/2h_fury_prot.png)

## Deep Prot:
Deep Prot loses a lot of the tools fury gives. In return, you get 10 defense and shield slam. Shield slam is extremely rage effecient.
 - Shield Slam - 250 static threat (think of this like unmitigated damage) + 342-358 damage + block value
   - Block value is the block number on gear + str * .5
   - 8/8 Wrath gives +27 block value, not counting str

### 1h
DPS: 312
![1h Deep Prot](/images/1h_deep_prot.png)

### DW
DPS: 464
![DW Deep Prot](/images/2h_deep_prot.png)

## Some real world bloodthirst damage numbers for ThreatDream and Beatus:

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
