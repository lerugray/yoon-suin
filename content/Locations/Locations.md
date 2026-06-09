---
type: locations-index
publish: true
---

# Locations

Every named place in the campaign, organized by geography. See
[[Adventure Log]] for the chronological play record; see
[[Chronicle]] for the running story.

## Geography map

Also see the [[Maps/Yellow City — Current State.canvas|Yellow City Current-State canvas]] for a geography-of-relationships view.

<details open>
<summary>Geography map</summary>

```mermaid
flowchart TB
  PurpleLand["The Purple Land"]
  Yellow["Yellow City<br/>(metropolis)"]
  Old["Old Town<br/>(ruined, south)"]

  Copper["Copper Ghetto<br/>raid in Turn 01"]
  Canal["Canal Quarter"]
  Safe["Canal Quarter Safehouse<br/>cell base"]
  Spice["Spice-Factor District<br/>Uvaris's beat"]
  Vellum["Vellum Lane"]
  Amber["Amber Moth Tea House<br/>Vellum Lane"]
  Merchant["Merchant Quarter"]
  Cart["Cartulary of Three Bells<br/>unexplored"]
  Ward["Ward of the Salt Shore"]
  Tidal["Tidal Mark<br/>offerings, twenty-two years"]

  PurpleLand --> Yellow
  PurpleLand --> Old
  Yellow --> Copper
  Yellow --> Canal
  Canal --> Safe
  Yellow --> Spice
  Spice --> Vellum
  Vellum --> Amber
  Yellow --> Merchant
  Merchant --> Cart
  Old --> Ward
  Ward --> Tidal
```

</details>

## Inside the Yellow City

- [[Yellow City]] — *the metropolis; caste society of the Purple Land.*
- [[Copper Ghetto]] — *the cell's old meeting place; raided in [[Turn 01]].*
- [[Canal Quarter]] — *the cell's current refuge.*
  - [[Canal Quarter Safehouse]] — *the cell's base.*
- [[Spice-Factor District]] — *Uvaris's beat.*
  - [[Vellum Lane]]
    - [[Amber Moth Tea House]] — *Uvaris's morning haunt; Hamech extracted in [[Turn 07]].*
- [[Merchant Quarter]] — *home of the Cartulary.*
  - [[Cartulary of Three Bells]] — *unexplored archive.*

## Beyond the city walls

- [[Old Town]] — *south, ruined; site of the [[Salt Shore Disturbance]].*
  - [[Ward of the Salt Shore]] — *Vothrog's current location.*
    - [[Tidal Mark]] — *the offerings, the old crab-man, the recognition.*

## Dataview index (renders inside Obsidian only)

```dataview
TABLE WITHOUT ID
  file.link as "Place",
  kind as "Kind",
  parent as "Parent"
FROM "Locations"
WHERE type = "location"
SORT parent ASC, file.name ASC
```

## See also

- [[Events/Salt Shore Disturbance|The Salt Shore Disturbance]] —
  *the event that shaped the southern landscape and Cheth's silence.*

## How to add a new location

When the campaign visits somewhere new:

1. Create `Locations/<Place>.md` with this frontmatter:
   ```yaml
   ---
   type: location
   name: <Display Name>
   parent: "[[Yellow City]]" # or another parent location
   kind: <quarter|street|safe-house|archive|tea-house|ritual-site|...>
   publish: true
   ---
   ```
2. Wikilink it from the relevant turn note and from this landing page.
3. Add a node + edge to the Mermaid geography map above if the
   place is load-bearing.

