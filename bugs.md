"Cannot build [{non-[Barracks]} {non-[Armory]} {non-[Walls]} {non-[Castle]} {non-[ConvertFilter]}] buildings <in [in this city] cities>", does not work when applied to a building. Puppeted does work
- "Shown while unbuilable" spelled wrong
- Unbuildable - "Blocks from being built, possibly by conditional. However it can still appear in the menu and be bought with other means such as Gold or Faith." Yet it disables buying thing with gold or faith.
- Neither "Costs [2] [Culture] per turn" nor "Costs [2] [Culture] per turn when in your territory" does anything on Fungal Bloom
- Stale link in https://yairm210.github.io/Unciv/Modders/Mods/: https://github.com/yairm210/Unciv-mod-example/blob/master/Removing%20Things/jsons/ModOptions.json The master branch of Unciv-mod-example does not contain the path Removing Things/jsons/ModOptions.json.
- Gaining a Great Prophet does not complete the city state quest for it if you consume it the same turn you get it.


- AI won't purchase unbuildable buildings? at least not this. It will build it if  <for [Human player] Civilizations>is added.
    {
        "name": "Willing Convert - Warrior",
        "uniqueTo": "Cult of the Eternal End",
        "cost": 0,
        "uniques": [
            "Costs [90] [Converts] <(modified by game speed)>",
            "Can be purchased for [0] [Gold] [in all cities]",
            "Free [Warrior] appears",
            "Only available <before discovering [Civil Service]>",
			"[+5 Production] <for [AI player] Civilizations> <hidden from users>",
            "Unbuildable <hidden from users>",
            "Shown while unbuilable <before discovering [Civil Service]>",
            "Will not be displayed in Civilopedia",
            "ConvertFilter <hidden from users>",
            "Suppress warning [unique \"ConvertFilter]",

            "Remove [Willing Convert - Warrior] [in this city] <hidden from users>"
        ]
    },


### Forgotten and Gold costs
- `Cost increases by [amount] per owned city does not affect purchase cost.` Maybe intentional, but might want to add it to the documentation
- `May buy [Technology Building] buildings with [Faith] for [2] times their normal Production cost` IS affected by purchase cost
- `Can be purchased with [Gold] [in all cities]` scales with production, and does increase per owned city. But adding `Unbuildable` drops it's cost from 230 Gold to 30 Gold, and 60 to 0 Faith on quick (presumably production cost = 0 base +5*0.67 from 1 city). Basically: This unique IS affected by the flat exttra build cost, but Unbuildable seems to drop its base cost to 0.
    - Actually, it works properly when explicitly setting the `cost: 100` field. It seems like Unbuildable just removes the autodetect from tech functionality

	{
		"name": "Buy Animal Husbandry",
		"uniqueTo": "Forgotten",
		"maintenance": 0,
        "hurryCostModifier": 50,
        "uniques": [
			"Unsellable", "Unbuildable", "Cannot be purchased<for [AI player] Civilizations>",
			"Can be purchased with [Gold] [in all cities]", // This scales with production
			"Will not be displayed in Civilopedia",
			"Technology Building",
			"Remove [Technology Building] [in all cities]<after turn number [1]>",
			"Cost increases by [5] per owned city",
			"Discover [Animal Husbandry]",
			"Only available <before discovering [Animal Husbandry]>"
			],
        "requiredTech": "Agriculture"
    },