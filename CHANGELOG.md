# Changelog

## v0.2.1-alpha (2026-11-20)
First playtest fixes. Start new games with it: Insight rules changed.

- **Insights fixed and reworked** (from the first playtest: they fired late, in bunches, "due to constructing Monument", and even for techs already researched):
  - Checked at the **start of every turn**, and only for techs you haven't researched yet. No more Insights (or Star Gazers / House of Wisdom bonuses) for known techs.
  - An Insight now makes its tech **cheaper to research** instead of adding progress. You can earn it long before you research the tech; nothing is wasted, and the research cost shows the discount.
  - A short **"Insight!" popup** tells you which tech got cheaper and why.
  - **Science pace back to roughly vanilla:** Insights are now **33%** (Babylon 50%) and techs cost **+33%** (was +25%). About 20 of the easiest conditions are harder (Masonry ← a Palisade, Civil Service ← capital at 10 population, Education ← 3 Academy Quarters, Architecture ← 6 Quarters, Fertilizer ← 3 Windmills…).
  - Known quirk: while you research a tech with an Insight, the tech screen shows every tech with that discount (the research itself is correct).

## v0.2.0-alpha (2026-11-20)
Built on v0.1.0-alpha. Start new games with it: rules changed, so ongoing v0.1 multiplayer games should finish on v0.1.

- **Great People meet Quarters**: Academy, Market, Artisan Quarters and Sacred Groves give 1 Great Scientist / Merchant / Engineer / Artist point per turn, and +2 to their yield for each adjacent Great Person improvement. Cluster your Great People around your Quarters.
- **Liberty and Freedom fixes**: Citizenship also gives +1 Happiness per Quarter; Meritocracy −10% unhappiness from population (was −5%); Constitution also +2 Culture per Great Person improvement.
- New wonders: **Grand Bazaar** (Guilds: Market Quarter tiles +2 Gold +1 Culture), **Palace of Versailles** (Economics: Golden Ages 25% longer, Golden Age focus twice as strong), **Crystal Palace** (Scientific Theory: one extra Legacy in every later era).
- First-time explanations for human players: a welcome popup on turn 1, and one the first time Imperial Strain or War Weariness appears.
- **How to play** guide in English and Spanish (`HOW_TO_PLAY.md`, `HOW_TO_PLAY.es.md`).
- Insights now cover **every era**: 58 more techs (78 in total; only Agriculture and Future Tech have none), many tied to Quarters and other new systems (Guilds ← Artisan Quarter, Architecture ← own 4 Quarters, Gunpowder ← 5 victories, Nanotechnology ← own 12 Quarters…). The +25% tech cost now applies in every era.
- New event **Casus Belli** when you declare war: *War Fervor* (new units +15 XP for 8 turns) or *Blitz* (+1 Movement for land units for 3 turns), each +2 War Weariness, or *Propaganda* (pay 60 Gold, −5 War Weariness).
- New event **Expedition** when you discover a natural wonder: *Survey* (Science), *Pilgrimage* (Faith + Culture) or *Tall Tales* (Gold); bigger from the Renaissance on.
- New event **Unrest** at −5 Happiness or worse (15-turn cooldown): *Martial Law* (+2 Happiness in garrisoned cities, −10% Production, no rebels, 10 turns), *Concessions* (15 Gold per city: +1 Happiness per city, 10 turns) or *Ignore them* (50% chance of rebels).
- Beliefs pass: weak and situational beliefs buffed (Faith Healers, God of War, Monument to the Gods, Goddess of Love, God of the Open Sky, Fertility Rites, Liturgical Drama, Religious Art, Reliquary). Peace Loving and World Church now count your own followers too, so they work in 1v1.
- New beliefs: **Star Gazers** (pantheon: every Insight also gives Faith), **Holy Groves** (follower: Sacred Grove tiles +1 Faith +1 Culture), **Warrior Monks** (follower: new military units +10 XP), **Pax Dei** (founder: War Weariness recovers faster, Culture per follower city while at peace).

## v0.1.0-alpha (2026-11-20)
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
