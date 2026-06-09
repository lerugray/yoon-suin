---
type: vault-index
publish: true
---

# Ray's Solo Campaigns

A vault of solo tabletop RPG campaigns, played and chronicled in
[mission-companion](https://github.com/lerugray/mission-companion)'s
RPG mode.

## Active campaigns

### [[Campaign|Whitehack/Yoon-Suin/Echo Resounding]]

> *Yoon-Suin's caste society. The Year of the Wandering Crane. A
> slug-man Heretic-Scholar in the vein of Thomas Müntzer.*

A solo Whitehack campaign set in [Yoon-Suin](http://monstersandmanuals.blogspot.com/p/yoon-suin.html),
threaded with the dominion-and-faction tools of *An Echo Resounding*
and the dynastic flavor of *Romance of the Three Kingdoms*. The
player character is **[[Vothrog|Vothrog the Wise]]**, a slug-man
Heretic-Scholar preaching that the divine spark resides in every
body regardless of species or caste — a protocommunist anabaptist
tuned to a setting of caste-locked god-emperors and opium-flooded
slums.

> **Where things stand at the end of [[Turn 16]]:** Vothrog has
> carried the news back to the cell and sent [[Selindi]] and
> [[Tuket]] to the Cartulary of the Three Bells. After a night's
> rest and a morning's provisioning, he stands at the merchant-
> quarter river-steps with [[Krah-Moh]] and [[Pav]] — and a
> salt-shore-blooded woman waiting on an honest answer before
> she'll travel with them. The road south begins.

**Read in order:**

1. [[Campaign]] — the seed: system, setting, character concept.
2. [[Chronicle]] — the running summary. Read this for the story so far.
3. [[Adventure Log]] — the full play record, turn by turn, with dice
   and all. Sixteen turns and counting.

---

## How this vault is organized

| Folder | Contents |
|---|---|
| Root | [[Campaign|Campaign seed]], [[Chronicle|Chronicle]], [[Adventure Log|Adventure Log index]]. |
| [[Turns/Turns|Turns]] | One note per ❖ turn (Turn 01 … Turn 16). |
| [[Characters/Characters|Characters]] | One note per named NPC; grouped by faction; relationship diagram. |
| [[Locations/Locations|Locations]] | One note per named place; geography hierarchy. |
| [[Events/Salt Shore Disturbance|Events]] | Historical events the campaign keeps circling. |
| Maps | A current-state JSON Canvas, scene paintings. |
| Portraits | Character portrait paintings. |
| Excalidraw | Editable Excalidraw drawings — [[Cell Relationships.excalidraw|Cell Relationships]], [[Yellow City Geography.excalidraw|Yellow City Geography]], [[Campaign Arc — Road South.excalidraw|Campaign Arc — Road South]]. |

## How play actually happens

Vothrog's story is generated turn-by-turn through conversation with
an LLM running inside mission-companion's RPG mode. The GM is a
prompt template; the dice are real (rolled in-app); the chronicle
gets compacted automatically when the log runs long. The result is a
campaign that survives across days/weeks without me needing to keep
the whole state in my head.

Every turn is one ❖ in the [[Adventure Log]]. **Sixteen turns in as
of this publish.**

---

```dataview
TABLE WITHOUT ID
  file.link as "Most recent activity",
  turn as "Turn"
FROM "Turns"
WHERE type = "turn"
SORT turn DESC
LIMIT 3
```

*(Dataview renders inside Obsidian. On the published site, the
read-in-order list above is the canonical entry point.)*
