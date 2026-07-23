# OSRS TCG — Card Collection Removal Audit

Audited `src/main/resources/Card.json` @ `main` (44a9dd6) — **6,376 cards**.
Classified from live OSRS Wiki page categories (fetched per-card), not keyword matching.
Item IDs are from OSRS Wiki infoboxes.

**349 cards recommended for removal.** Tradeable items are excluded — they stay live in
the main-game economy (54 cards, listed at the end).

| Category | Cards |
|---|---|
| Event / holiday / anniversary | 286 |
| Diango reclaimables | 12 |
| Limited-time / discontinued / unobtainable | 31 |
| Temporary gamemodes (DMM / Leagues) | 23 |
| Quest items | 0 — all 10 matches are permanently obtainable |
| **Total** | **349** |

---

## 1. Event / holiday items (286)

```
// 2005 Halloween event
6722 // Zombie head

// 2013 Christmas event
10507 // Reindeer hat

// 2013 Halloween event
11847 // Black h'ween mask
9920 // Jack lantern mask
9921 // Skeleton boots
9922 // Skeleton gloves
9923 // Skeleton leggings
9925 // Skeleton mask
9924 // Skeleton shirt

// 2014 Birthday event
11918 // Birthday present
11919 // Cow mask
23987 // Crystal halberd (variants: 24125)
795 // War ship

// 2014 Christmas event
12897 // Antisanta's coal box
6865 // Blue marionette
6866 // Green marionette
6864 // Marionette handle
6867 // Red marionette
6822 // Star bauble (variants: 6824, 6826)
6840 // Tree bauble (variants: 6842, 6844)

// 2014 Easter event
1037 // Bunny ears
4565 // Easter basket

// 2014 Halloween event
12845 // Grim reaper hood
12836 // Grim reaper's diary
12837 // Grim robe
12842 // Scythe sharpener
12838 // Will and testament

// 2015 April Fools
13188 // Diango's claws

// 2015 Christmas event
13343 // Black santa hat
13344 // Inverted santa hat

// 2015 Easter event
13186 // Volatile mineral

// 2016 April Fools
13679 // Cabbage cape
13681 // Cruciferous codex

// 2016 Birthday event
13655 // Gnome child hat

// 2016 Christmas event
20836 // Giant present
20834 // Sack of presents

// 2016 Easter event
13664 // Bunny legs
13665 // Bunny paws
13663 // Bunny top

// 2016 Halloween event
20779 // Hunting knife

// 2017 Birthday event
21211 // 4th birthday hat
21209 // Birthday balloons

// 2017 Christmas event
21866 // Santa suit
21872 // Vault key
21863 // Wise old man's teleport tablet

// 2017 Easter event
21239 // Crunchy chocolate mix
21246 // Sea salt
21240 // Wester banana
21249 // Wester fish

// 2017 Halloween event
21722 // Diving helmet
21720 // Jonas mask
21712 // Spectral potion
21714 // Tattered book

// 2018 Birthday event
22316 // Prop sword

// 2018 Christmas event
22713 // Star-face
22717 // Tree skirt
22715 // Tree top

// 2018 Halloween event
22687 // Church lectern
22692 // Clown bow tie
22695 // Clown gown
22689 // Clown mask
22701 // Clown shoes
22698 // Clown trousers
22686 // Dead person
22684 // Eek (variants: 8485)

// 2019 Birthday event
23105 // Brewer's folly
23104 // Cook's letter
23106 // Vyvin's wine

// 2019 Christmas event
24428 // Green gingerbread shield
24430 // Red gingerbread shield
24441 // Scaperune teleport

// 2019 Easter event
23448 // Bunnyman mask

// 2019 Halloween event
24325 // Pumpkin lantern
24327 // Skeleton lantern
24298 // Smoke powder
24323 // Spookier boots
24321 // Spookier gloves
24315 // Spookier hood
24317 // Spookier robe
24319 // Spookier skirt
24313 // Spooky boots
24311 // Spooky gloves
24305 // Spooky hood
24307 // Spooky robe
24309 // Spooky skirt

// 2020 Birthday event
24525 // Cat ears
24527 // Hell cat ears

// 2020 Christmas event
25314 // Giant boulder
25286 // Mouldy sawdust

// 2020 Easter event
24539 // '24-carat' sword

// 2020 Halloween event
24975 // Headless head
24977 // Magical pumpkin
24992 // Spider snack

// 2021 Birthday event
25502 // Banana cape
25500 // Cursed banana

// 2021 Christmas event
26290 // Clean full helm
26286 // Clean platebody
26288 // Clean platelegs
26312 // Festive elf hat
26310 // Festive elf slippers
26284 // Pink stained full helm
26280 // Pink stained platebody
26282 // Pink stained platelegs
26314 // Snowman ring

// 2021 Easter event
25604 // Gregg's eastdoor
25606 // Propeller hat

// 2021 Halloween event
26252 // Ad coupon
26247 // Pumpkin pie
26256 // Ugly halloween jumper

// 2022 Birthday event
26645 // Banana pizza
26649 // Skis
26600 // Tiny fish

// 2022 Christmas event
27566 // Christmas jumper
27588 // Festive games crown
27561 // Light beer
27578 // Nutcracker boots
27576 // Nutcracker hat
27580 // Nutcracker staff
27572 // Nutcracker top
27574 // Nutcracker trousers
27558 // Sack of coal
27568 // Snow goggles & hat

// 2022 Easter event
26919 // Big bucket
26920 // Big bucket of camel milk
26925 // Cooler
26939 // Crate ring
26937 // Easter hat
26916 // Special hot sauce
26917 // Special super hot kebab
26931 // Tanning wheel
26934 // Wooden pole

// 2022 Halloween event
27463 // Treat cauldron (variants: 27467, 27471)
27479 // Witch boots
27481 // Witch cape
27473 // Witch hat
27477 // Witch robes
27475 // Witch top

// 2022 Pride event
27039 // Beautiful yellow pansy seed
27035 // Flower crown (variants: 27143, 27147, 27151, 27155)

// 2023 Birthday event
27820 // 10th birthday balloons
27812 // 10th birthday cape
27806 // Bob the cat slippers
27804 // Cake hat
27810 // Dragon candle dagger
27801 // Dwarf cake
27799 // Gnome cake
27802 // Gnome child backpack
27818 // Gnome child plush
27800 // Goblin cake
27814 // Jad plush
27808 // Jad slippers
27822 // Oldschool jumper (variants: 27823, 27824, 27825, 27826, 27827)
27828 // Silver partyhat
27816 // Stray dog plush

// 2023 Christmas event
28786 // Icy jumper
28788 // Snowglobe helmet

// 2023 Easter event
27873 // Eastfloor spade
27871 // Giant bronze dagger
27875 // Nest hat

// 2023 Halloween event
28601 // Cobweb cape
28603 // Spider hat (variants: 28607, 28611)
28671 // Web cloak

// 2023 Pride event
28128 // Love crossbow
28126 // Poet's jacket
28116 // Rainbow jumper (variants: 28119, 28121, 28123, 28125)

// 2024 Christmas event
30491 // Dog boots
30487 // Dog disguise
30489 // Festive scarf
30479 // Present box hat (variants: 30483)

// 2024 Easter event
29433 // Book of egg
29443 // Egg priest mitre
29441 // Egg priest necklace
29437 // Egg priest robe
29439 // Egg priest robe top

// 2024 Halloween event
30234 // Halloween scarecrow
30232 // Scarecrow shirt

// 2024 Pride event
29489 // Rainbow cape (variants: 29493, 29497, 29501, 29505)
29507 // Rainbow crown shirt (variants: 29510, 29512, 29514, 29516)

// 2025 Birthday event
30648 // Classic imp hood
30646 // Classic imp tail

// 2025 Christmas event
32930 // Beer belly sweater
32934 // Christmas dinner
32932 // Jad jumper
32928 // Lovley jubbly bib
32926 // Serving platter

// 2025 Easter event
30722 // Carrot costume body
30726 // Carrot costume gloves
30720 // Carrot costume hat
30724 // Carrot costume tights
30717 // Raisins

// 2025 Halloween event
31231 // Grim reaper bottoms
31233 // Grim reaper gloves
31229 // Grim reaper top
14815 // Spooky chair (variants: 31225)
31227 // Spooky pumpkin lantern
31224 // Spooky scarecrow
31223 // Spooky wall lamp

// 2026 Easter event
33146 // Scribbled notes

// 20th Anniversary event
25328 // 20th anniversary boots
25326 // 20th anniversary bottom
25334 // 20th anniversary cape
25330 // 20th anniversary gloves
25322 // 20th anniversary hat
25332 // 20th anniversary necklace
25324 // 20th anniversary top
25338 // Gnome child icon
25336 // Gnome child mask

// 25th Anniversary event
33086 // 25th anniversary 5x5 hat
33080 // 25th anniversary helmet
33084 // 25th anniversary skeleton tabard
33082 // 25th anniversary warrior tabard

// Christmas corrupt cluefest
20838 // Corrupted helm
20846 // Corrupted kiteshield
20840 // Corrupted platebody
20842 // Corrupted platelegs
20844 // Corrupted plateskirt

// Event rewards
12896 // Antisanta boots
12895 // Antisanta gloves
12893 // Antisanta jacket
12892 // Antisanta mask
12894 // Antisanta pantaloons
20773 // Banshee mask
20777 // Banshee robe
20775 // Banshee top
11862 // Black partyhat
6856 // Bobble hat
6857 // Bobble scarf
13182 // Bunny feet
22719 // Candy cane
11019 // Chicken feet
11021 // Chicken head
11022 // Chicken legs
11020 // Chicken wings
19695 // Clue hunter boots
19697 // Clue hunter cloak
19689 // Clue hunter garb
19691 // Clue hunter gloves
19693 // Clue hunter trousers
12958 // Cow gloves
12959 // Cow shoes
12956 // Cow top
12957 // Cow trousers
12600 // Druidic wreath
21214 // Easter egg helm
7927 // Easter ring
22351 // Eggshell platebody
22353 // Eggshell platelegs
13286 // Gravedigger boots
13287 // Gravedigger gloves
13285 // Gravedigger leggings
13283 // Gravedigger mask
13284 // Gravedigger top
21354 // Hand fan
19687 // Helm of raedwald
27428 // Hood of ruin
19699 // Hornwood helm
27440 // Infinite money bag
6858 // Jester hat
6859 // Jester scarf
13203 // Mask of balance
23093 // Ornate boots
23099 // Ornate cape
23091 // Ornate gloves
23101 // Ornate helm
23095 // Ornate legs
23097 // Ornate top
11863 // Rainbow partyhat
21314 // Rainbow scarf (variants: 28109, 28111, 28113, 28115)
4566 // Rubber chicken
12891 // Santa boots
12890 // Santa gloves
12888 // Santa jacket
12887 // Santa mask
12889 // Santa pantaloons
21849 // Snow imp costume body
21857 // Snow imp costume feet
21855 // Snow imp costume gloves
21847 // Snow imp costume head
21851 // Snow imp costume legs
21853 // Snow imp costume tail
6860 // Tri-jester hat
6861 // Tri-jester scarf
21859 // Wise old man's santa hat
6862 // Woolly hat
6863 // Woolly scarf
4079 // Yo-yo (variants: 2261, 2262, 2263, 2264, 2265)

```

---

## 2. Diango reclaimables (12)

Toys/commemoratives reclaimable from Diango (his permanent shop stock excluded).

```
// Diango reclaimable
13218 // Amur leopard toy
25840 // Banana hat
11705 // Beach boxing gloves
11708 // Cursed goblin bow
11707 // Cursed goblin hammer
11709 // Cursed goblin staff
12727 // Goblin paint cannon
13216 // Lion toy
27645 // Mystic cards
21695 // Runefest shield
13217 // Snow leopard toy
13215 // Tiger toy
```

---

## 3. Limited-time / discontinued / unobtainable (31)

```
// Discontinued content
20525 // Adamant arrow pack
24565 // Antique emblem (variants: 24569, 24573, 24577, 24581)
11340 // Barbarian skills
31172 // Battlehat
24609 // Blighted bind sack
24611 // Blighted snare sack
26704 // Blighted wave sack
12561 // Bloodthirst rockslug   [Monster card]
20523 // Catalytic rune pack
13514 // Dark manuscript (variants: 13516, 13518, 13520, 13522)
20524 // Elemental rune pack
22818 // Fish chunks
13429 // Fresh fish
24277 // Mysterious emblem (variants: 24281, 24285)
26549 // Portable waystone
4654 // Rowdy Guard   [Monster card]
20607 // Rune arrow pack
3062 // Strange box

// Discontinued content, Unobtainable items
12656 // Junk

// Unobtainable items
8858 // 18lb shot
8859 // 22lb shot
9106 // Astral tiara
4614 // Broken plate
25280 // Essence pack
11427 // Fish vial
9595 // Hazelmere's book
30939 // Mind mender
4238 // Puddle of slime
11848 // Rancid turkey
1460 // Soul talisman
11525 // Wimpy feather

```

---

## 4. Temporary gamemode items — DMM / Leagues (23)

```
// Deadman Mode
13302 // Bank key (variants: 13304, 13306)

// Deadman Mode, Deadman seasonal items
12746 // Archaic emblem (variants: 12749, 12751, 12753, 12755)
30689 // Trinket dust

// Deadman: Annihilation, Deadman seasonal items
15547 // Big Evil Chicken   [Monster card]
15553 // I DSCIM YOU   [Monster card]
15557 // TzTok-Jad-Rek   [Monster card]
15558 // Zemouregal Summon (variants: 15560, 15562)   [Monster card]

// Deadman: Annihilation, Deadman: Apocalypse, Deadman: Armageddon, Deadman seasonal items
12452 // Giant goblin   [Monster card]

// Deadman: Annihilation, Deadman: Armageddon, Deadman seasonal items
13663 // Magic Mark   [Monster card]
13664 // Ranging Ro   [Monster card]

// Demonic Pacts League
33338 // Demonic slayer helmet
33218 // Knapsack
28771 // Searing boots
33231 // Soul shard

// Demonic Pacts League, Raging Echoes League
30340 // Crystal dagger
30357 // Forager's pouch

// Demonic Pacts League, Raging Echoes League, Shattered Relics League, Trailblazer Reloaded League
26551 // Arcane grimoire

// Shattered Relics League
27645 // Mystic cards
26549 // Portable waystone

// Trailblazer Reloaded League
12561 // Bloodthirst rockslug   [Monster card]

// Twisted League
28595 // Twisted extract
24370 // Twisted slayer helmet
28630 // Twitcher's gloves

```

---

## 5. Quest items — 0 recommended for removal

Wiki `Category:Quest items` matches exactly 10 cards; all are permanently obtainable
and permanently kept, so none qualify: `Helm of neitiznot` (GE-tradeable),
`Guthix`/`Saradomin`/`Zamorak staff` (Mage Arena, repeatable), `Keris partisan`,
`New crystal shield`, `Captain's log`, `Current duck`, `Mayor of catherby`, `Cowbell amulet`.

The category means *quest-associated*, not *quest-exclusive*.

Quest NPCs/monsters (212 cards) are out of scope for an items audit, and the same rule
applies — most are permanently killable (`Dharok the Wretched`, `Demonic gorilla`).

---

## Kept: tradeable — NOT for removal (54)

```
// Event
1055 // Blue halloween mask
1042 // Blue partyhat
11910 // Chocolate strawberry
962 // Christmas cracker
981 // Disk of returning
1961 // Easter egg
1053 // Green halloween mask
1044 // Green partyhat
1989 // Half full wine jug
11171 // Newspaper
1959 // Pumpkin
1046 // Purple partyhat
1057 // Red halloween mask
1038 // Red partyhat
1050 // Santa hat
1048 // White partyhat
1040 // Yellow partyhat

// Diango
2524 // Black toy horsey
2520 // Brown toy horsey
2526 // Grey toy horsey
2522 // White toy horsey

// Limited
20430 // Ancient magicks tablet
7804 // Ancient mjolnir
31454 // Ball of cotton
7226 // Burnt chompy
1867 // Burnt pitta bread
2154 // Equa toad's legs
1411 // Farmer's fork
29098 // Not meat
2245 // Odd batta
2094 // Odd cocktail (variants: 2098)
2197 // Odd crunchies
2173 // Odd gnomebowl
2203 // Rock-climbing boots
2158 // Seasoned legs
2156 // Spicy toad's legs
2160 // Spicy worm
6053 // Spirit roots

// Gamemode
33305 // Demonic axe ornament kit
33342 // Demonic quill
33296 // Demonic sceptre
33302 // Demonic skin contract
33308 // Demonic staff ornament kit
????? // Demonic tallow
33311 // Demonic trident ornament kit
30432 // Echo venator bow ornament kit
33365 // Impish whistle
26424 // Shattered banner
26517 // Shattered cane
26528 // Shattered cannon ornament kit
24413 // Twisted banner
24395 // Twisted cane
24466 // Twisted horns
24391 // Twisted trousers

```
Tradeability is taken from the OSRS Wiki, which overrides `Card.json` where they disagree.
That happens exactly once in the flagged set: `White toy horsey` is marked `tradeable: true`
in `Card.json` but has no Tradeable/GE category on the wiki (unlike its black/brown/grey
siblings), so it stays on the removal list.

`Black h'ween mask` is **not** here — unlike the red/green/blue masks it is an untradeable
2013 event reward, so it stays on the removal list. League/DMM entries are tradeable only
*within* their gamemode; parked here per your call.

---

## Reviewed and NOT flagged (false positives)

Permanent NPCs that merely appeared in an event — keep:

- `Anja` — 2018 Halloween event
- `Cow31337Killer` — 2017 Birthday event, 2018 Birthday event
- `Gnome child` — 2016 Birthday event, 2017 Birthday event, 2023 Birthday event
- `Hengel` — 2018 Halloween event
- `Mad melvin96` — 2019 Halloween event
- `Mugger` — 2017 Birthday event
- `Ram` — 2021 Easter event
- `Sir Tiffy Cashien` — 2016 Birthday event
- `Wise Old Man` — 2014 April Fools, 2014 Birthday event, 2015 Halloween event, 2017 Birthday event, 2017 Christmas event, 2018 Birthday event, 2019 Birthday event, 2020 Birthday event, 2021 Easter event, 2022 Birthday event, 20th Anniversary event

Also excluded: Diango's permanent shop stock (`Oculus orb`, `Spinning plate`, `Chronicle`, `Teleport card`).

---

## Note on the `questItem` field

`Card.json` carries a `questItem` boolean on 5,151 of 6,376 cards — it is `false` on **every**
card. Dead weight today; repopulatable from wiki `Category:Quest items` or osrsbox-db
`quest_item` (the latter is per-item-ID, so it needs an ID-level join, not a name match).