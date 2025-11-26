
# PF1

| Field | Value |
|:---|:---|
| Creature Type | creatureType |
| Custom Creature Type | creatureType |
| Current HP | attributes.hp.offset |
| Max HP | attributes.hp.max |

Here's a script macro to setup some default colors for the different creature types found in pf1

```js
const bloodSheetData = {
  aberration: "#b527d5d5",
  animal: "#a51414d8",
  construct: "#5f4d39d5",
  dragon: "#40ab26d8",
  fey: "#b304add8",
  magicalBeast: "#b71e46d8",
  humanoid: "#a51414d8",
  monstrousHumanoid: "#810808d8",
  ooze: "#0000cc6d8",
  plant: "#195d09d8",
  undead: "#260000d8",
  outsider: "#b304add8",
  vermin: "#195d09d8",
};

game.settings.set("splatter", "BloodSheetData", bloodSheetData);
```

# PF2E

1. Module settings:

| Field | Value |
|:---|:---|
| Creature Type | traits.value |
| Custom Creature Type | traits.value |
| Current HP | attributes.hp.value |
| Max HP | attributes.hp.max |

2. Script macro to set default colors. (Remember that *Automatic Blood Color* must be enabled in the module's settings.) Based on data taken 2025/08/17

```js
const BloodSheetData = {
  blight: "#5b4d0dcc",
  duskwalker: "#999BC9D8",
  ghul: "#444559D8",
  kovintus: "#a51414d8",
  paaridar: "#a51414d8",
  sporeborn: "#B8AC93D8",
  suli: "#a51414d8",
  shade: "#260000D8",
  anugobu: "#a51414d8",
  centaur: "#a51414d8",
  ghoran: "#0C2B04D8",
  hantu: "#0C2B0400",
  ikeshti: "#a51414d8",
  Lilu: "#520A0AD8",
  merfolk: "#a51414d8",
  munavri: "#a51414d8",
  oread: "#767E9CD8",
  stheno: "#a51414d8",
  tanggal: "#4A1057D5",
  undine: "#003DB8D5",
  vanara: "#a51414d8",
  wraithvine: "#A12596D5",
  wyrwood: "#A1259600",
  formian: "#B9D158D5",
  grioth: "#8E86E1D8",
  herald: "#8E86E100",
  inevitable: "#8E86E100",
  palinthanos: "#8E86E100",
  sedacthy: "#590B0BD8",
  shabti: "#a51414d8",
  spriggan: "#590B0BD8",
  sylph: "#3F3CD6D5",
  bugbear: "#780F0FD8",
  graveknight: "#2B0000D8",
  morlock: "#A53F3FD8",
  skulk: "#C24A4A36",
  titan: "#a51414d8",
  darvakka: "#260019D8",
  siktempora: "#a51414d8",
  asura: "#B71E46D8",
  azarketi: "#a51414d8",
  catfolk: "#a51414d8",
  dhampir: "#a51414d8",
  nagaji: "#a51414d8",
  vishkanya: "#C95421D8",
  anadi: "#2164C935",
  grippli: "#a51414d8",
  hobgoblin: "#7A0F0FD8",
  seugathi: "#870BA3D5",
  aesir: "#a51414d8",
  azata: "#55A6CDD5",
  hryngar: "#B33636D8",
  kami: "#B3363600",
  nindoru: "#8F1737D8",
  oni: "#a51414d8",
  serpentfolk: "#a51414d8",
  skelm: "#a51414d8",
  agathion: "#60D0E8D5",
  alchemical: "#73F30FD8",
  div: "#b71e46d8",
  kaiju: "#8A0000D8",
  phantom: "#8A000000",
  qlippoth: "#b71e46d8",
  tengu: "#a51414d8",
  aeon: "#424242D5",
  wraith: "#000000D5",
  angel: "#FFFA7DD8",
  changeling: "#a51414d8",
  drow: "#6E14A5D8",
  urdefhan: "#1457D9D8",
  astral: "#463078d5",
  acid: "#32b432f2",
  rakshasa: "#a5141400",
  caligni: "#260000D8",
  fetchling: "#4D4D4DD8",
  lizardfolk: "#a51414d8",
  velstrac: "#691128D8",
  archon: "#5DB6E0D5",
  dero: "#690265D8",
  illusion: "#69026500",
  psychopomp: "#08010100",
  sahkil: "#b71e46d8",
  boggard: "#a51414d8",
  ratfolk: "#a51414d8",
  ethereal: "#a5141400",
  time: "#a5141400",
  nymph: "#b304add8",
  protean: "#343791D5",
  sprite: "#CC05C5D8",
  werecreature: "#a51414d8",
  daemon: "#a51414d8",
  mummy: "#240404D8",
  troll: "#080101D8",
  arcane: "#a51414d8",
  wight: "#240800D8",
  dinosaur: "#a51414d8",
  genie: "#a5141400",
  xulgath: "#A54444D8",
  dream: "#A5444400",
  gremlin: "#CF05C8D8",
  golem: "#CF05C800",
  hag: "#a51414d8",
  clockwork: "#a5141400",
  soulbound: "#a5141400",
  occult: "#40ab26d8",
  electricity: "#ffff00d8",
  ghost: "ffff0000",
  vampire: "#360606D8",
  devil: "#a51414d8",
  kobold: "#a51414d8",
  devil: "#a51414d8",
  ghoul: "#260000d8",
  celestial: "#55a6cdd5",
  skeleton: "#55a6cd00",
  cold: "#55a6cdd5",
  ooze: "#f3900fd8",
  orc: "#a51414d8",
  zombie: "#260000d8",
  divine: "#a5141400",
  air: "#92cfffd1",
  fungus: "#5D4E46D8",
  giant: "#541e1ed8",
  demon: "#a51414d8",
  aquatic: "#a51414d8",
  water: "#345985D8",
  earth: "#5F3D18D5",
  plant: "#195d09d8",
  incorporeal: "#195d0900",
  fire: "#FF5C00D5",
  amphibious: "#a51414d8",
  fey: "#b304add8",
  dragon: "#40ab26d8",
  elemental: "#737373B1",
  beast: "#a51414d8",
  aberration: "#b527d5d5",
  fiend: "#b71e46d8",
  construct: "#5f4d39d5",
  mindless: "#a51414d8",
  animal: "#a51414d8",
  undead: "#260000d8",
  humanoid: "#a51414d8",
};

game.settings.set("splatter", "BloodSheetData", BloodSheetData);};

game.settings.set("splatter", "BloodSheetData", BloodSheetData);
```

# ALIEN

1. Module settings:

| Field | Value |
|:---|:---|
| Creature Type | type |
| Custom Creature Type | type |
| Current HP | header.health.value |
| Max HP | header.health.max |

2. Script macro to set default colors: red for human blood, white-ish for synthetics' fluid, and green for xenomorph's acid. (Remember that *Automatic Blood Color* must be enabled in the module's settings.)

```js
const BloodSheetData = {
  character: "#a51414b0",
  creature: "#1dbb02b0",
  synthetic: "#f7f7f7b0",
};

game.settings.set("splatter", "BloodSheetData", bloodSheetData);
```

# DAGGERHEART

1. Module settings:

| Field | Value |
|:---|:---|
| Creature Type | ancestry.name |
| Custom Creature Type | attribution.source |
| Current HP | resources.hitPoints.value |
| Max HP | resources.hitPoints.max |
| Wounds System | TRUE / CHECKED`|

> NOTE: Since adversaries dont generally use ancestries, I set the custom Creature Type to the attribution. (Top right 3 dots in character sheet -> Configure attribution -> SOURCE) this is a big ol' hack and if someone knows any better way of solving this, be my guest.

2. All ancestries from Daggerheart CORE as well as THE VOID - Mixed ancestries obviously would need to be configured manually.
If you want companions to have splats aswell, use the source attribution "hack" alike with adversaries

```js
const bloodSheetData = {
// Celestial/Energy-based
  Aetheris: "#c0c0c0d8", // Silvery-White/Radiant
  Astran: "#1e0b3dd8",   // Deep Violet/Cosmic dust
  Crystalline: "#606060d8", // Grey/Clear mineral-like
  Emberkin: "#ff6600d8", // Glowing Orange/Fire
  Glimmerkin: "#ffff00d8", // Yellow/Sparkling Joy
  Infernis: "#cc0000d8", // Dark Red/Heat/Brimstone
  Oneiroi: "#9370dbd8", // Medium Purple/Dream-like
  Skykin: "#87ceebc0",   // Light Blue/Airy
  Sylph: "#b0e0e6c0",    // Powder Blue/Near-transparent
  Umbral: "#000000d8",   // Black/Shadow
  Voldur: "#add8e6d8",   // Pale Blue/Frost

  // Humanoid/Mammalian
  Carchari: "#a51414d8", // Standard Red
  Centaur: "#a51414d8", // Standard Red.. you know the drill..
  Drakona: "#a51414d8",
  Dwarf: "#a51414d8",
  Elf: "#a51414d8",
  Giant: "#a51414d8",
  Gnome: "#a51414d8",
  Halfling: "#a51414d8",
  Human: "#a51414d8",
  Kapibara: "#a51414d8",
  Katari: "#a51414d8",
  Kitsune: "#a51414d8",
  Rattan: "#a51414d8",
  Simiah: "#a51414d8",

  // Aquatic/Reptilian/Amphibian/Insectoid "Special"
  Arachne: "#000000d8",  // Black/Hemolymph (Insectoid/Spider)
  Drow: "#22003dd8",   // Very Dark Purple/Venous
  Faerie: "#9acd32d8",   // Greenish-Yellow/Plant sap-like
  Firbolg: "#694a34d8", // Brownish-Red/Earthy
  Grotesque: "#694a34d8", // Brownish Red
  Loxodon: "#4d2919d8", // Dark Brown/Thick
  Naga: "#336600d8",     // Dark Green/Serpentine
  Orc: "#708238d8",     // Olive Green/Iron-rich
  Ribbet: "#006400d8",   // Dark Green/Amphibian
  Vespine: "#9acd32d8",  // Greenish-Yellow/Hemolymph (Wasp/Bee)

  // Other/Construct/Unique
  Clank: "#808080c0",     // Grey/Oils or hydraulic fluid (translucent)
  Fungril: "#ff00ffd8",   // Magenta/Spores/Mycelial fluid
  Galapa: "#4b5320d8",    // Khaki/Shell-based/Thick
  Gargoyle: "#484848c0",  // Dark Grey/Stone particles
  Gelatinoid: "#00bfff99",// Deep Sky Blue/Translucent Ooze
  Sylvanwood: "#228b22d8",// Forest Green/Sap/Chlorophyll
  Tidekin: "#0000ff99",   // Blue/Sea water (somewhat translucent)

};

game.settings.set("splatter", "BloodSheetData", bloodSheetData);
```
