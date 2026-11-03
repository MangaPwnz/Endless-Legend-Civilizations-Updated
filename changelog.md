# Changelog

## v1.0.0

Update uniques

## v1.0.1

fix various bugs coming from misspellings

## v1.0.2
Add a separate Mykara nation which implements the original Creeping Presence mechanic.

## V1.0.3
Rebalance Mykara.
- Add extra bonuses on adopting policies in the Liberty tree
- Spore Bearers (Settlers) now gain extra charges and cost more per era
- Less consumption of food by Unemployed pops after discovering Biology
- +4 faith from ANY natural wonder in their territory.
- Fungal Bloom:
    - now scales with techs instead of granting all its bonuses in the early game
    - every 3 Fungal Blooms produce 1 unhappiness
    - now only gains control of unowned tiles

## V1.0.4
- Add Mycelial network (sub unique)
    - Mykara roads on Fungal Blooms cost more.
    - Mykara units gain increase movement speed from Fungal Bloom, and can research teleport (paradrop).
- Spore Bearers now gain 5 charges and extra cost starting from Industrial era
- Clean up and simply formatting for all of Mykara's abilities

## V1.1.0
Lots of stuff
- Overhaul Cult of the Eternal End
- Rebalance Mykara
    - Fungal Blooms now increase policy cost
    - Spore Bearers also gain extra movement speed starting from the Industrial era
    - Remove faith from Natural Wonders
    - Other minor tweaks
    - bug fix: Science from strategic resources works properly now
- Add icons for most things
- Other minor changes
- Disable a few civilizations with bugs

## V1.1.1
Add Roving Traders as an alternative version of the Roving Clans.

## V1.1.2
Bugfix: Stockpiles now actually scale with game speed
Add Fanatic, a UU for Cult of the Eternal End
- increase cost of "Willing" Converts to 100.
- Fanatic Converts now give +1/+2/+3 Faith per 2 pop in capital after building 2/4/6.
- UA no longer provides +1 Faith per 2 pop in capital

## V1.1.3
Reimplement the Cultist's inability to adopt the Liberty policy tree. Now it should be compatible with other mods which edit the Liberty tree.
Fix broken icons
Cultists:
- nerf: 15% City strength in Converted villages
- improve readability in the Civilopedia
Mykara - Fungal bloom (nerfed):
- remove production from plains (Metal Casting)
- makes the tile it's built on unworkable
- can now only be built in unowned tiles to stop players from ruining AI tiles
- no longer replaced by automated units for Humans
- improve readability in the Civilopedia
Mykara - Mycelial network:
- now only works on tiles without roads and railroads
- no longer increases maintenance cost of roads/railroads

## V1.1.4
Bugfixes:
- Fix Personalities overflowing on the starting screen for some civs
- Fix Broken Lords losing population from starvation every turn

Forgotten:
- Rebalance tech cost. All techs no longer cost a constant 200 gold.
- Add a small quest to gain Ziema Adya, a hero unit with her own promotion tree

Cultists:
    Buffs:
    - Add start bias Avoid Tundra, Avoid Snow.
    - Now unlocks their "Converts" UB at Calendar instead of Theology
    - Converted village gives 1 Happiness, resulting in a net -3 Happiness per new city founded.
    - "Willing Converts" building cost reduced by 25%
    - "Willing Converts" gives -3 Happiness (from -4)
    - Gains additional benefits from the Honor tree
    - Gains additional benefits from Piety tree
    - Converted Villages can now grow their borders

    Other:
    - Rebalanced Stockpiles. Production and Science Stockpiles also give a flat bonus regardless of era.
    - Fanatic Converts: gives more Faith early, but less late. Gaining an extra founder belief is locked behind Piety
    - Fix: Converted Villages giving starving warnings despite being at 1 population
    - Fix: Could previously buy any building in a Puppeted city the first turn.

    Nerfs:
    - Stockpile gain from razing cities: 3 per turn -> 2 per turn
    - Removed bonus Faith from conquering Holy Cities
    - Fanatic Converts now reduces happiness by 3

## V1.1.5
Forgotten has been overhauled. The goal is to make them less aggression and gold-focused and lean into their stealth and information theme:
- Science to Gold conversion reworked and greatly nerfed to allow buffing the espionage theme. Previously the conversion happened in each city, giving ridiculous amount of base gold from library, population and public schools, as well as extra % gold modifiers from university and reasearch lab. This left them weak early but with high late-game gold generation. Now it happens globally at turn end, keeping the science and gold modifiers split.
- Forgotten no longer gains extra gold from conquering cities or barbarian camps
- Forgotten now gains 1 gold per civilization (including city-states and themselves) discovered
- New UU, Myst. A stealthy *Scout*-type unit which replaces horseman and does not require horses. Amazing pillager
- "Pillaging costs no movement" replaced with +100% yield from pillaging
- No longer gains a free spy from Agriculture
- Can build Information Brokers improvement inside enemy borders, which provides extra spies

Cultists:
- Clarify tooltip

Roving Traders
Buffs:
- Added specialist slot for their UBs, the same as the ones they replace
- Kassai can always move after attacking

Other
- Fix being unable to build National College in Capital due to being unable to construct
- Rename Bardic Schools to Bardic Academy

Nerfs:
- - Each Bardic Academy (Opera House) and Network Academy (University) now increase maintenance cost of ALL other "Academy" buildings by 10%, multiplicatively (i.e. scaling exponentially)
- Caravan School (Library) is now a pre-requisite for Network Academy

