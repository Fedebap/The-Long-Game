# Changelog

## v0.1 (unreleased)
Baseline: Unciv **5.0.1** *Civ V – Gods & Kings* ruleset (`yairm210/Unciv@82edba7`).

- Imperial Strain meter (anti-snowball): tech, policy and city-unhappiness costs scale with how far you're ahead in cities.
- War Weariness meter, speed-scaled.
- Comebacks: Rally the Nation event, Call to Arms (Mobilization), Reconstruction when a war ends, Desperate Defence.
- Early game: Palisade building, stronger base city strength.
- Insights: 20 Ancient and Classical techs get a 40% boost for doing something thematic (shown on the tech). Those techs cost 25% more.
- Quarters (light districts): Academy, Market, Sacred Grove, Artisan and Garrison. A city building places a tile that yields without a citizen, plus adjacency bonuses. University, Bank, Workshop and Grand Temple need their Quarter.
- Legacies: each era (and your first city) offers a choice of 3 permanent bonuses, plus a free tech ("Rising Star") for civs behind the tech average.
- Events: Conquest (plunder, integrate or garrison a captured city), Alliance perks on friendship or defensive pact, Golden Age focus.
- Military: Slinger (cheap ancient ranged), Battering Ram and Siege Tower (support units, +30%/+40% vs cities for adjacent melee, capturable), Field Medic (healing support), Mercenary Company (gold-only), morale (Shaken / Emboldened), unit upkeep +5% per era.
- Wonders: Great Bath (War Weariness heals fast), Hadrian's Wall (enemies spend +1 movement in your land), House of Wisdom (Insights also give Culture). Each World Wonder you own makes the next one 5% slower to build.
- Balance: University +25% (was 33%), Research Lab +40% (was 50%), Naval Tradition also gives Gold in coastal cities.
- Civilopedia: a welcome page and articles for every new system.
- Fortunes (separate optional extension): 10 random events (plague, harvest, drought, gold rush, comet, pirates, mercenaries, scholar, great fire, heresy), about one every 25 turns.
- Very Quick game speed (0.5×).
- Balance: Piety no longer exclusive with Rationalism, plus Piety buffs. Honor opener reworked.
- Roster: 6 Gods & Kings civs kept (Rome, Korea, Egypt, Aztecs, Byzantium, Babylon). The 28 others and their unique units/buildings/improvements were removed.
- New civs: Mapuche (anti-leader), Vietnam (defence), Mali (trade and Market Quarters), Poland (two Legacies per era).
- Base civ reworks: Babylon = Insights (60%, no free Great Scientist at Writing), Korea = specialists + Academy Quarters, Rome halves Strain, Egypt +50% Artisan Quarters, Byzantium +50% Sacred Groves, Aztecs recover from War Weariness faster.
- Tooling: `tools/check.py` static checker + CI. Engine tests (18) verify the systems inside Unciv 5.0.1's own game logic.
