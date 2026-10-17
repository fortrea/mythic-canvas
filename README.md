# Mythic Canvas

Living worlds of mythic creatures, drawn entirely in code. Five self-contained HTML5 canvas pages: four cursor scenes and Dragon World, a whole realm to explore. No build step, no dependencies: open any `.html` file in a browser.

| Page | Scene | Creatures |
|---|---|---|
| `bone-dragon.html` | Heavenly mountains: karst peaks with pagodas, floating temple islands, celestial gate, sea of clouds, aurora | Bone dragons that grow celestial skins and beards (original) |
| `dragon-realistic.html` | Heavenly mountains (same scene) | Realistic, richly scaled dragons with painted heads; the mantle can be toggled on or off |
| `dragon-world.html` | A wide side-view realm that grows more heavenly from left to right: Ashen Wilds, Ember Highlands, Gilded Spires, Celestial Terraces and Mount Olympus | Five castes (Common, Middle, High, Emperor and the one Dragon King), 28 elements with their own breath, nests, eggs, hatchlings and a full life cycle (drag to explore, scroll to zoom, click a dragon or nest) |
| `mushroom-swarm.html` | Enchanted toxic forest: giant mushrooms, twisted trees, witch's hut, fog, fireflies | Poisonous mushroom creatures that ripen into toxic colors |
| `celestial-maidens.html` | Hillside village and old town: castle, church, windmill, clock tower, street lamps | Winged celestial maidens in flowing gowns |

![Preview](assets/preview.png)

## Cursor scenes (bone dragons, realistic dragons, mushrooms, maidens)

- **Cursor rings**: heads spread evenly on rings around the cursor and always face it, leaving the centre clear.
- **Tap / click**: the whole swarm lunges and fires particles at the cursor.
- **Idle formations** (2.5 s without moving): Vortex, Orbits, Infinity Chase, Rose Bloom, Supernova/Burst. Switches every 9 s.
- **Life cycle**: newcomers fly in from the edges; skins / colours bloom over time; at the end of their lifespan they ascend and leave a star (or a glowing mushroom on the forest floor).
- **Day–night cycle**: one full day every 160 s (sunrise, noon, golden hour, sunset, dusk, night) with moving sun and moon, clouds, birds, and windows and lanterns that light up at night. The current time is shown bottom-left.
- Respects `prefers-reduced-motion`.

## Dragon World

- **Five castes from left to right**: Ashen Wilds (Common), Ember Highlands (Middle), Gilded Spires (High), Celestial Terraces (Emperor) and Mount Olympus, home of the one Dragon King. Dragons only live in their own realm or a lower one.
- **28 elements** in tiers, each with its own breath: classic (fire, water, ice, lightning…), light and dark, and beyond (void, cosmic, time, gravity, chaos, dream). The King breathes Aether.
- **Life cycle**: flying, landing, perching, brooding, sleeping at night, eggs, hatchlings that follow their parent, ageing, and ascension to the stars.
- **Controls**: drag to explore, scroll or pinch to zoom, minimap and caste track to travel, click a dragon or nest for details, Roar and Breathe buttons.

## Run locally

Open `index.html` in a browser, or serve the folder with Node.js (no install needed):

```bash
npx serve .
```

Then open the address it prints (usually http://localhost:3000).

## Publish with GitHub Pages

Settings → Pages → Source: *Deploy from a branch* → Branch: `main` / root. The landing page is `index.html`.
