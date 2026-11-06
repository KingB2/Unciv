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
- **Merlin (or Lailoken)** must be pickable.
- Candidate pool to research: Taliesin, Michael Scot, Albertus Magnus, Roger Bacon, Nicolas Flamel, Paracelsus, John Dee, Abe no Seimei, Zhang Daoling, Hildegard of Bingen, Rasputin…

### Resource: Mana
- **One magic resource: Mana.**
- **Icon: a burning skull.**
- Used to **cast spells** in game.
- Some **units require Mana** to build.

### Spells
- **Summon Storm:** summon a natural disaster (a storm) that damages anything within it.
  - Open: does it drift? Can it hurt your own side? Can rivals tell it was you? Does it leave anything behind?
- **Principle: spells change with context.** How a spell behaves depends on who you're playing, the era, and your techs and civics. (E.g., an early storm might be wild; later techs or civics could let you steer or disguise it.)

### Cults
- Over the course of the game, you can **join different cults** for bonuses and other benefits.
- Inspired by Civ VI Secret Societies and governors.
- Open: one cult at a time or several? Permanent, or switchable (e.g., at era changes)? Are cults joined as a nation, or are they people you place, like governors?

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
- Civ VI **Disasters** game mode
- Civ VI **Secret Societies** game mode
- Civ VI **Zombie** game mode
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
- **Thin places:** spots on the map where the Veil is cracked; Mana is harvested there. Powerful but risky to build near.
- **Veil as shared world health:** spending magic thins it; low Veil → more disasters ("Breach surges") and incursions (zombie-mode analogue). *Designer not sold.*
- **Religion as "what is the Breach?":** each faith answers that question (heaven, hell, Faerie, a wound…) and so sets how its people treat magic.
- **Secret Societies → wizard orders:** lodges, covens, cabals offering forbidden power with their own agendas.
- **Espionage → magical spycraft:** scrying, stealing spells, sabotage, triggering incursions in rival lands.
- **City-states → beings from beyond the Breach:** fae courts, elder peoples.
- **Era 4 → Thaumaturgic Revolution:** Mana-burning industry.
- **Era 5 → synthetic magic:** salvation or final mistake.
- **Story spine:** wonder → industry → trying to replace the thing that changed everything.

---

## Technical Notes
- Plan: use **Unciv** (open source, MPL 2.0) as the engine template, reshaped into its own game.
- This fork is from ~late 2021 — **update to current Unciv** before building.
- Mobile: keep map size, faction count, and per-turn simulation in check. Lots of content is fine.
- All art and music is made by the designer. **No AI-generated art.**
