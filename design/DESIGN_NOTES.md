# Wizard 4X — Design Notes

*Working title: none yet.*
*A living document. "Settled" means decided for now — anything can be revisited.*

---

## The Pitch (so far)

A historical 4X where you rule a **wizard nation**. In the Dark Ages, a hole tore open in the Veil — **the Breach** — and magic, fairies, and things like aliens from another dimension came pouring through. Magic is public and everywhere. Practically all of history after Rome is wizards.

**Inspirations:** Castle Falkenstein, Deadlock (for feel — the world itself is original).
**Mechanical inspirations:** Civilization (esp. Civ VI), Victoria, Age of Empires, Humankind / Civ VII (era switching).

**Why make it:** an excuse to learn history and the occult, and to make art and music.

---

## Roadmap (what to design next)
Alternating fun and slog:
1. ~~Leaders~~ (done: 16)
2. **Spells** (fun): signature spells for a few leaders, then work out the general rules of spellcasting from them
3. ~~Civ list~~ (done: 20). Civ uniques still to do: each civ's earthly identity (land, buildings, unique units)
4. **Cults** (fun): what each cult does, per era
5. **The core loop** (slog): where mana comes from, the Veil, how you win
6. **Era changes**: what happens at each transition
7. **First playable build** in Godot (a tiny one)

---

## Settled

### Start
- The game begins at **the moment the Breach opens**.

### Eras (5)
| # | Era | Rough dates (adjustable) |
|---|-----|--------------------------|
| 1 | Post-Roman / Early Medieval | ~500–1000 |
| 2 | Late Medieval / Early Renaissance | ~1000–1450 |
| 3 | Late Renaissance / Baroque | ~1450–1700 |
| 4 | Enlightenment / Industrial / Modern | ~1700–1945 |
| 5 | Mid-20th Century / Contemporary / Future | ~1945 onward |

*Note: Era 4 covers a lot of ground — keep an eye on it.*

### Leaders
- Leaders are historical and legendary figures who were (in this world, actually) magicians.
- **Global and timeless**, like Civ.
- **The rule:** not entirely fictional, not entirely ordinary. Two kinds qualify:
  1. **Reality grown into legend:** a real person with myth or magic attached (Charlemagne, Elizabeth Báthory, Houdini).
  2. **Legend grown from reality ("the Merlin Protocol"):** a literary invention built on a probably-real seed (Myrddin Wyllt).
- **Timeline:** leaders should have lived after the Breach (~500 onward).
- Careful: avoid founders and prophets of living religions; saints are a judgment call.

**Decided: roster (16)**
- Myrddin Wyllt (Merlin)
- Charlemagne
- Dante Alighieri
- Ursula Southeil (Mother Shipton)
- Elizabeth Báthory
- Sundiata Keita: prophesied at birth; his epic is a war against the sorcerer-king Soumaoro Kanté.
- Nehanda (Charwe Nyakasikana): care. National heroine of Zimbabwe; spirit mediumship is a living tradition.
- Jabir ibn Hayyan
- Kublai Khan
- Abe no Seimei
- Seondeok of Silla
- Lin Moniang: care. Worshipped today as Mazu by millions; portray her as the mortal woman before deification, with respect.
- Manco Cápac
- Tenskwatawa (the Shawnee Prophet): signature: darkening the sun (the 1806 eclipse). A complex figure (also led witch hunts). Care: seek a Shawnee perspective; avoid fraud or noble-savage clichés.
- Marie Laveau: handle with care. Revered in Louisiana Voodoo, a living religion; avoid the "sinister Voodoo" trope; ideally get a reader from that tradition.
- Harry Houdini

**Considering**
- William Shakespeare, Alexander I of Russia, Cagliostro, Bhoja of Malwa (South Asia)
- Other Taoist Immortals: Lü Dongbin, Zhang Guolao (best documented: a biography in the official Tang histories), and/or the Eight Immortals as a cult. Care: still venerated in Taoist folk religion.
- More women: Nzinga of Ndongo, Himiko, Catherine de' Medici, Olga of Kiev, Hildegard of Bingen, Semiramis
- Merlin-types: Thomas the Rhymer, Taliesin, Nicolas Flamel, Rabbi Loew (the Golem of Prague), Gilgamesh, the Pied Piper of Hamelin, King Arthur, Pope Joan (may be fully fictional)
- Others from earlier lists: Virgil, Gerbert of Aurillac, Michael Scot, Albertus Magnus, Roger Bacon, Paracelsus, Nostradamus, Comte de Saint-Germain, Vseslav of Polotsk, Owain Glyndŵr, Harun al-Rashid, Ahmad al-Buni, Soumaoro Kanté, Abe no Seimei, En no Gyōja, Ge Hong, Choe Chiwon, Nezahualcoyotl, Pachacuti, Moctezuma II

**On the fence**
- Wovoka: religious prophet of Indigenous movements still meaningful to living communities; would want consultation first.
- Timothy Leary: recent; his estate likely controls commercial use of his name and likeness.

**Cut**
- John Dee (replaced by Mother Shipton), Vikramaditya (too early), Timur (replaced by Kublai Khan), Prester John (too fictional), He Xiangu, Faust, Topiltzin Quetzalcoatl (trimming men / thin records), Dihya (al-Kahina) (thin magic sourcing), Qin Shi Huang (before the Breach; replaced by Abe no Seimei), Grigori Rasputin, Maria Prophetissa (before the Breach), Kamehameha I, Vlad Dracula (replaced by Elizabeth Báthory), Hasan-i Sabbah (myth, but not magic: better as the face of a spy/assassin cult or a spy adventurer), Jeanne d'Arc (replaced by Mother Shipton: Andegavia winning the Hundred Years' War complicates her)

### Leaders are immortal wizards
- Leaders are **immortal (or near-immortal) wizards** who rule for the whole game.
- Like **Civ III**, leaders **look different every era** (new portrait/outfit per era).
- **Any leader can be picked**, regardless of when they lived historically.
- **Any leader can lead any civ.** Two levels of customization at the start (leader + civ), plus a big shifting one through the game (cults).
- **Leaders have unique spells**, in addition to the spells you research.
- Art note: 5 eras means up to 5 looks per leader.

### Civs don't transition; cults do
- **Civs stay the same all game.** The era-to-era transformation comes from **cults**: each era, your nation can take up a new cult.

### Civs
- **Random maps.** Every game is different.
- **Some civs can be alt-history nations**, e.g. an industrial-era Plantagenet realm, or Burgundy. Not a rule for all civs.
- **Civs can come from any era**, not only the first (the way Civ still lets you play America). No civ switching.
- **Nothing from before the 5th–6th century.** Civs aren't restricted to eras otherwise.
- Watch: don't drift into pure alt-history (Harry Turtledove). Civs should keep a real connection to real countries. The differences from real history come from **magic**.
- **Civs are nations,** thought of in a national sense (like Civ before Civ VII). **A civ doesn't change its face each era**: England just stays England.
- **The approach:** history, but different because of wizards. Familiar and strange aren't mutually exclusive. Not rule of cool; the list should have a subconscious rhythm, and gets **felt out** rather than built from a rule.
- Consideration: the leader roster is already full of deep cuts, so familiar civs may give players footing.
- **Reference: Civ V's roster by era** (all 43 civs, sorted by their leader's era): Ancient 4, Classical 5, Medieval (500–1450) 14, Early modern (1450–1700) 8, 1700–1945: 12, post-1945: ~0. Mapped onto our eras (34 post-500 civs): Era 1 ~15%, Era 2 ~26%, Era 3 ~24%, Era 4 ~35%, Era 5 ~0%. Civ avoids post-1945 nations almost entirely.
- **Reference: Civ VI's roster by era** (all 50 civs, sorted by each civ's original leader): Ancient 5, Classical 8, Medieval 16, Early modern 10, 1700–1945: 11, post-1945: 0. Mapped onto our eras (37 post-500 civs): Era 1 ~11%, Era 2 ~32%, Era 3 ~27%, Era 4 ~30%, Era 5 0%.
- **Both games averaged:** Era 1 ~13%, Era 2 ~29%, Era 3 ~25%, Era 4 ~32%, Era 5 ~0%.
- Rough target for a ~16–20 civ list: Era 1: 2–3, Era 2: 5–6, Era 3: 4–5, Era 4: 5–6, Era 5: 0–1 (a natural slot for invented or alt-history nations).
- **Process:** name every civ's three uniques first (breadth), then design abilities later, once the core loop (Mana, Veil, casting) exists to design against.
- **Civ uniques (structure):** every civ gets **one unique piece of infrastructure, one unique unit, and one unique magic unit.**
  - **A civ's magic unit is a unique Adventurer type.** Adventurers riff on fantasy adventuring parties (D&D-style classes) mixed with folklore, and it's all otherworldly. E.g., the Franks' Paladin, the Britons' Bard.
  - Open: is there also a civ ability? Are uniques tied to their historical era, or can they be speculative (magical alt-history)?
  - Resolved: leaders carry personal spells; civs carry their culture's magic through their unique Adventurer.
- **Civ list (20):** the Britons, the Franks, Andegavia, the Netherlands, Bavaria, Prussia, Spain, al-Andalus, the Papal States, Arabia, Mali, Ethiopia, India, China, Japan, the Mongols, Hawaii, Acadia, the Haudenosaunee, the Muisca.
  - **Pulled:** Jerusalem, the Paiute, Romania, Tibet, the Inca, the Ottomans, Antillea, Poland, Italy, Byzantium, the Rus', Greenland.
  - Why Acadia: Americans will want to play as themselves.
- **Civ details so far:**
  - **The Britons:** sub-Roman Britain, Roman-influenced Brythonic (Welsh, Cornish, Breton, and the classical Celts of England). Capital: Caerleon.
    - **Infrastructure: the Caer** (improvement; Welsh for a fort or fortified enclosure, as in Caerleon).
    - **Unit: the Breton** (unique settler; the real migration of Britons to Armorica, which became Brittany, in the 5th–6th centuries).
    - **Magic unit (Adventurer): the Bard.**
    - Considered: Gododdin Riders (rejected: the battle was a famous defeat); the Picts (current scholarship leans toward Pictish being a Brittonic language, though they were a separate people and often the Britons' enemies).
  - **The Franks** (renamed from Francia, to make the Lotharingian and Capetian connection clear): the Frankish kingdom and its dynasties, including West, East and Middle Francia. Capital: Aachen.
    - **Infrastructure: the Scriptorium** (Carolingian revival of learning). (Pfalz rejected: overlaps with the Caer.)
    - **Unit: the Scara** (Charlemagne's elite cavalry, his personal bodyguard).
    - **Magic unit (Adventurer): the Paladin.**
  - **Andegavia (Angevin):** a nation with a combined Anglo-French culture developed over centuries, a parallel to 18th–19th-century Britain and France. Real roots: the Anglo-Norman language, and Law French in English courts. Capital: Paris.
  - **The Netherlands:** grows out of the medieval and Renaissance Burgundians; named for the Low Countries because that's the culture that became nationally dominant. Look: somewhere between 17th-century Amsterdam and 19th-century Brussels. Capital: Brussels.
  - *(Pulled)* **Greenland:** Norse Greenland, including Vinland: "what if the Greenlandic golden age kept going." Consider a Norse–Inuit blended culture.
  - **The Netherlands:** *La Mourisque* (Tielman Susato, *Danserye*, Antwerp, 1551) / *Sur la route de Dijon* (French folk song; Dijon was Burgundy's capital)
  - **Prussia:** the Baltic Prussians; the Northern Crusades never destroyed them. A Baltic people, not German Prussia. (No Lithuania.)
  - **Bavaria:** home of the Illuminati and Neuschwanstein; chosen over "the Germans" or Austria.
  - **Acadia:** the America-equivalent; name still open (Orleans and Columbia also possibilities).
  - **The Papal States:** confirmed (over the Holy See); in the designer's head, also includes Naples (historically a papal fief for centuries).
  - *(Pulled)* **Antillea:** survivors of the Western Roman Empire who end up in the pre-Columbian Caribbean; may or may not survive the colonial era. Considerations: timing (Rome fell in 476, before the Breach, unless the Breach carried them); avoid a colonial story by making them refugees absorbed into a blended culture. Named after Antillia, the medieval legend of refugees who fled Iberia across the Atlantic to an island of Seven Cities (the Antilles are named after it).

### Resource: Mana
- **One magic resource: Mana.**
- **Icon: a burning skull.**
- Used to **cast spells** in game.
- Some **units require Mana** to build.

### Darkness (direction, details open)
- **The fog of war is dangerous, not just unseen.** Darkness is a threat.
- **Barbarians are monsters:** ogres and other creatures in the dark.
- A goal is to **keep the darkness at bay**: light fires, build watchtowers.
- **The Veil is a tile feature**, a layer on a tile like hills or vegetation.
- **Barbarian monsters spawn from Veils**, which can be anywhere, including near your cities. (In Civ, barbarians can't spawn within a set distance of cities; here they can.)
- **Founding a city automatically clears the Veil from the city's tile.** Everything else has to be cleared.
- **Fog of war in two steps:** unexplored (can't see) → explored but Veiled (can see, still dangerous) → cleared.
- **New Veil regions spawn in the fog of war at each era transition.** (So vision does matter: it doesn't stop monsters spawning from existing Veils, but it keeps new Veil from forming.)
- **Dedicated anti-monster techs, units and buildings** exist specifically to fight the barbarian monsters.
- Open: what does clearing take? Is there a reason *not* to clear one (e.g., it also yields Mana)?
- Ideas on the table: light as territory; light sources that advance by era (torches → lanterns → gaslight → electric → artificial-magic light); Tenskwatawa's eclipse temporarily brings the darkness everywhere; darkness could be the other side seeping through (a possible answer to what the Veil does).

### Breaches
- **The Breach is a physical place on the map, surrounded by Veil.**
- **There's one on every continent** (rather than a single one at the center of the map).
- **Units can interact with Breaches.**
- Each Breach is a gateway to unimaginable other planes of existence, where the fairies and other beings come from.
- **Breaches are NOT city-states** (no diplomacy with them). You can explore, trade and colonize. City-states are a separate thing.
- Ideas on the table: the Breach tore open once in 500 and its pieces fell on every continent; each Breach opens onto a different plane, perhaps shaped by that continent's folklore; adventurers travel through Breaches to trade and gather crafting ingredients.
- **Only adventurers can go through.** Entering triggers an **event chain**, like a Victoria exploration mission.
- **Rewards:** harvest Mana, get unique fairy units, other things.
- **Overuse has a price:** if a Breach is entered too many times in one era, it can spawn a **super-strong barbarian unit** (a "barbarian Giant Death Robot"), e.g. a dragon.
- **Later eras:** a Breach can be **claimed permanently by imperializing and colonizing the other plane.**
- **Breaches can be shut** for massive one-time bonuses. **Closing Breaches is likely a victory condition.**
- **The overuse counter is shared** by everyone using that Breach.
- Open: what exactly wins: closing all Breaches, most, or one per continent?
- Note: colonizing other planes in the imperial era will rhyme with real colonialism, and the roster includes anti-colonial leaders (Nehanda, Tenskwatawa). Worth designing on purpose (e.g., the planes resist).

### Mythology
- **Mythology is the non-player layer.** Fully mythic figures (gods, monsters, folk spirits) aren't leaders; they're city-states, incursion threats, wonders and cult patrons.
- Care with gods of living religions.

### Spells
- **How casting works (like launching a nuke, but weaker and with varied powers):**
  - Spells are cast within a **casting range** of a city (e.g., 6 tiles). The range **can be expanded**.
  - Within that range, you **target one tile**.
  - Each spell then has **its own radius** of effect around that tile.
- **Summon Storm:** summon a natural disaster (a storm) that damages anything within it.
  - Open: does it drift? Can it hurt your own side? Can rivals tell it was you? Does it leave anything behind?
- **Houdini (signature): the Escape.** Within a certain radius, all his units gain an extra turn of movement (but can't attack) and ignore zone of control.
  - Cast on a target tile within casting range; affects units within the spell's radius.
  - Open: does "can't attack" also block pillaging and capturing?
- **Lin Moniang (signature): Walk the Waves.** Select an area of units; they can move and attack on water tiles as if they were land. When the spell ends, units on water automatically embark.
  - Open: how long does it last?
  - Not chosen (could return as a passive or second spell): Calm the Storm, immediately ending a hurricane in your territory.
- **Principle: spells change with context.** How a spell behaves depends on who you're playing, the era, and your techs and civics. (E.g., an early storm might be wild; later techs or civics could let you steer or disguise it.)

### Cults
- Over the course of the game, you can **join different cults** for bonuses and other benefits.
- Inspired by Civ VI Secret Societies and governors.
- **Both layers:**
  - **Nation level:** your nation follows a cult, and can **switch to a new one each era** (ties into era switching).
  - **People level:** individual **cult members are placed in cities like governors** (e.g., a necromancer, an augur, a stormcaller).
- Open: how do the two layers interact? (E.g., does your nation's cult decide which members you can recruit? Can you hire members of other cults, at a cost or risk?)
- Idea on the table: cults as the **organization of magic** itself — each cult a school with its own spells.
- **Cult roster (first pass, what they do TBD):** Druids, Vampires, Templars, Headhunters, Cthulhu cultists, the Golden Dawn, the Masons, the Rosicrucians, Plague Doctors, and more.
- Possible era fit (historical "home" era, not decided):
  - Era 1: Druids
  - Era 2: Templars, Plague Doctors (Black Death)
  - Era 3: Rosicrucians
  - Era 4: Masons, Golden Dawn, Vampires (Gothic)
  - Era 5: Cthulhu cultists
  - Timeless: Headhunters
- **Cults are locked to their eras.**
- **Cults aren't exclusive:** several players can follow the same cult (how many may depend on the number of players).
- Open: what does sharing a cult mean between players? Allies, rivals, or both?
- Watch: roster is mostly European so far; a worldwide set of civs will want cults from other traditions too.

### Crafting (Alchemy)
- **Alchemy is part of a larger crafting system.**
- Discovering alchemy lets you **convert resources into other resources**.
- **Relics and great works can be crafted** by exchanging resources for them.
- Crafted items are **magic, so they carry big bonuses**.
- Crafted relics **provide bonuses in your cities the way resources do**.
- Open: where do rare ingredients come from? Are recipes known, or discovered?
- Idea on the table: rare ingredients come from dangerous or special places, especially **Breach expeditions**, plus monsters, city-states and trade.

### The Adventurer
- Instead of only building scouts, you can build an **adventurer** (inspired by Age of Empires).
- On death, the adventurer **returns to your capital after a cooldown**.
- The adventurer is the one who can **negotiate and collect** (e.g., rare crafting ingredients, deals).
- Adventurers **level up** and **change with the eras**, possibly as a player choice (e.g., keep a veteran vs. retrain into the new era's form).
- **Great People work this way:** Great People are adventurers.
- **Multiple types:** e.g., explorer, warrior, scholar.
- **Civ-unique adventurers:** e.g., **Paladins for the Franks**.
- Open: how many can you have at once? Does dying cost anything (e.g., losing what they carried)?
- Watch: lots of heroes = lots to control on a phone, and lots to draw. Probably cap how many are active.

### Blood Pacts
- **Blood pacts** can be added to **diplomatic agreements** for extra-powerful bonuses.
- Open: what happens if you break one?

### The Veil
- The Veil is **separate from Mana** — a whole-world mechanic, not a spendable resource.
- Icon idea: four-pointed star.

---

## Images the Game Should Deliver
*These came first — mechanics should serve them.*
- A **leader scene** of Merlin standing there.
- A **diplomacy screen** with a city-state of noble elves (original elves — no Tolkien names or lore).
- **Factories that run on magic** instead of steam.
- **Modern-day labs creating artificial magic.**
- **Cultist units** moving into another civ's territory.

---

## Things the Designer Loves (want in some form)
- Civ VI **Apocalypse** game mode (and Disasters)
- Civ VI **Heroes & Legends** game mode
- Civ VI **Secret Societies** game mode
- Civ VI **Zombie Defense** game mode
- **Religion** (Civ VI's was the most interesting, though it still fell short)
- **Espionage**
- **Era switching** (Civ VII / Humankind)
- **Governors**
- **Dynamic events** (Victoria III)

---

## Open Questions
- **Where does Mana come from?**
- **How is magic organized?** (schools, orders, sources — unclear)
- **The Veil as world health — not sold on it yet.** What *is* the Veil mechanically, if anything?
- **What came through the Breach, exactly?** Beings, a place, a force — or all three?
- What is religion *about* in a world where magic is real and public?
- How does era switching work — what transforms, what carries over?
- How do you win?
- Game name.

---

## Ideas on the Table (proposed, NOT decided)
- **Mythology lore (open):** possible lore: the Veil was always thin enough to leak, which inspired the old myths, and the Breach made them real; or the beings from beyond wear the masks of human stories. Care with gods of living religions.
- **Thin places:** spots on the map where the Veil is cracked; Mana is harvested there. Powerful but risky to build near.
- **Veil as shared world health:** spending magic thins it; low Veil → more disasters ("Breach surges") and incursions (zombie-mode analogue). *Designer not sold.*
- **Religion as "what is the Breach?":** each faith answers that question (heaven, hell, Faerie, a wound…) and so sets how its people treat magic.
- **Secret Societies → wizard orders:** lodges, covens, cabals offering forbidden power with their own agendas.
- **Espionage → magical spycraft:** scrying, stealing spells, sabotage, triggering incursions in rival lands.
- **City-states → beings from beyond the Breach:** fae courts, elder peoples. (Note: Breaches themselves are not city-states.)
- **Era 4 → Thaumaturgic Revolution:** Mana-burning industry.
- **Era 5 → synthetic magic:** salvation or final mistake.
- **Story spine:** wonder → industry → trying to replace the thing that changed everything.

---

## Languages (open questions)
- **The Netherlands / Burgundy:** a French-speaking Burgundian court ruling a mostly Dutch-speaking population (like Belgium today). Would the state still call itself Burgundy? Precedent: Brandenburg's realm took the name "Prussia" from a peripheral territory because that's where the royal title was. Language likely bilingual: Dutch (Flemish) majority, French court and south (Walloon).
- **Andegavia:** probably not one merged language; more likely French as the prestige language and English as the vernacular, with English becoming even more French than it really is. Real models: Anglo-Norman, Law French, and the Norman languages still spoken in Jersey and Guernsey.
- **Prussia:** a Baltic language with East German influence. Real evidence: the 16th-century Old Prussian catechisms already show heavy German borrowing.
- Where language shows up in the game: city name lists, unit names, possibly leaders speaking their own language (as in Civ VI).

## Music (early ideas)
- Civ themes drawn from real traditional music (designer is a musician; anthropology interest):
  - **The Britons:** *Pais Dinogad* (Old Welsh lullaby, 7th–8th c., in the margins of *Y Gododdin*; only the words survive, so the melody would be composed)
  - **Acadia:** *Simple Gifts* (Shaker, 1848) / *La danse de Mardi Gras* (Cajun)
  - **Andegavia:** *Le Roy Engloys* (Bayeux Manuscript) / the *Agincourt Carol* (15th c.)
  - **The Franks:** *Rolandskvadet* (Norwegian medieval ballad about Roland)
  - **Prussia:** *Pirs man is Danskos* / *Dāncau nūs angzdrīkikis* / *Zeminnika kweitākedi* (check: likely modern Old Prussian revival songs, so probably under copyright). Public-domain alternative to set to music: the Basel Epigram (1369), the oldest Old Prussian text, a drinking toast.
  - **The Haudenosaunee:** *Ho, Ho, Watanay* / *Waho; hiya ne* ("Just a Song"). Care: only use social songs, never ceremonial ones; ideally check with Haudenosaunee singers.
- Idea: like Civ VI, one theme per civ, re-arranged for each of the five eras.
- Watch: the old tunes are public domain, but specific modern arrangements and recordings aren't (e.g., Copland's *Simple Gifts* in *Appalachian Spring*).

## Neighbors on the Shelf
- **Age of Wonders** (esp. AoW4): closest relative. Shares wizard rulers, mana, spells, heroes, monster lairs, and magic "tomes" researched over time. Differs: pure invented fantasy (no real history, no historical leaders, no Breach-to-present eras), tactical battle maps. Our darkness/Veil layer is our own.
- Others in the genre: Master of Magic, Endless Legend.
- Takeaway: same genre, not the same game. Avoid copying specifics.

## Technical Notes
- **Engine: Godot. Fresh start** — not built on Unciv.
  - Why: the design has grown beyond Civ's shape, the graphics in the designer's head need a whole new rig, Godot's text-based project files suit AI-assisted building, and it's free and open source with a growing pool of human developers.
- **A human developer will review the code before any release.** No all-vibe-coded release.
- Release path (a ladder): private build → friends playtest → free demo on itch.io → Steam Early Access and/or Google Play. Android + PC first; iPhone later if ever.
- Disclose AI coding help per store rules at the time; all art and music are human-made.
- Mobile: keep map size, faction count, and per-turn simulation in check. Lots of content is fine.
- All art and music is made by the designer. **No AI-generated art.**
