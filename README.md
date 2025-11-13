# 🧠 BD-LSC: Bi-Directional Lexical Semantic Change
### A Dataset and Benchmark for Tracking Word Meaning Evolution in Slang and Standard English

---

## 🔍 Overview
**BD-LSC** (Bi-Directional Lexical Semantic Change) is a benchmark dataset for analyzing how word meanings **gain**, **lose**, or **remain stable** over time — across both **standard English** and **slang**.  
It introduces a **bi-directional annotation scheme**, capturing the complex evolution of senses across **three time periods (T1, T2, T3)**.

Unlike traditional lexical semantic change datasets that classify only “change” vs “no change,” BD-LSC explicitly distinguishes:
- 🟢 **Sense Gain (SG)** – new meanings emerge  
- 🔴 **Sense Loss (SL)** – old meanings fade  
- ⚪ **Stable (NC)** – meanings remain unchanged  

---

## 🧱 Dataset Composition

| Period | Years | Source | Description |
|:------:|:------|:--------|:-------------|
| **T1** | 1980–1999 | CCOHA / COHA | Late 20th-century formal English |
| **T2** | 2000–2009 | COHA | Early 21st-century transitional English |
| **T3** | 2010–2020 | Twitter, Urban Dictionary | Modern slang and online language |

**Data Sources:**
- **Standard English:** COHA, CCOHA, Oxford English Dictionary (OED)  
- **Slang Sources:** SlangSD, Urban Dictionary, Green’s Dictionary of Slang  
- **Annotation:** 3 expert linguists (Cohen’s κ ≈ 0.9 across periods)

---



## 💬 Target Words and Change Types

The BD-LSC dataset contains **79 target lemmas**, each annotated across **T1–T2–T3** for sense change and accompanied by examples of both **standard** and **slang** usage.

---

### Overview of Target Words and Semantic Change Labels (BD-LSC)
This dataset presents an extended lexical semantic change resource that includes both **standard** and **slang** usages of English words across three time periods (T1–T3).  
Each entry preserves *all raw senses* from the source sheet (“Words_lemmas_after_Filter”) and includes semantic change labels across temporal intervals.

---

### 🔍 Label Legend
| Symbol | Meaning |
|:-------|:--------|
| 🟢 Gain | New sense(s) or extended usage appeared |
| 🔴 Loss | Older sense(s) declined or disappeared |
| ⚪ Stable | No significant change across the period |

---

### 📘 Overview of Target Words and Semantic Change Labels (BD-LSC)

| Word | All Standard Meanings | All Slang Meanings | T1–T2 Label | T1–T3 Label | T2–T3 Label |
|:------|:----------------------|:-------------------|:-------------|:-------------|:-------------|
| abc | First three letters of the English alphabet. | American Born Chinese / Australian-born Chinese; American Broadcasting Company | ⚪ Stable | 🟢 Gain | 🟢 Gain |
| artichoke | A vegetable | The act in which someone uses their teeth on a penis, during a blowjob, in a scraping motion, similar to how one would eat an artichoke; the vagina; an old woman; a man; to smoke (a pipe) | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| eat | consuming food | to give oral pleasure to a female; make money; to rob someone; to defeat or destroy; to annoy | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| atm | Automated Teller Machine | “At The Moment”; “Ass To Mouth” | 🔴 Loss | 🟢 Gain | 🟢 Gain |
| bam | Used to imitate the sound of a hard blow or to convey abruptness | Scottish slang “Below Average Mentality”; exclamation “Bam!”; to have sexual intercourse | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| battery | A device to store electrical energy | Jamaican slang for gang sex; a man using performance-enhancing drugs during sex | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| beetle | An insect | A flashy young woman; to hurry away; Volkswagen car | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| bing | Heap of ore; search engine | A dose of drugs; solitary confinement cell; money | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| blender | Kitchen appliance | Fingering motion during sex; euphemism for sex; aggressive person | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| bmw | Car brand | “Black Man’s Wish”; “Be My Wife”; “Black Magic Woman” | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| bom | Brother; friend | Bill of materials; exclamation of joy; attractive person | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| bot | Robot; automatic program | Incompetent gamer; AI persona; buttocks; homosexual act | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| bouncer | Large man employed to keep order | On-off partner; liar; large object | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| breather | Brief pause; vent for air | Smoker in meetings (“loud breather”) | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| brownie | Chocolate dessert | Marijuana edible; airhead person; referring to brown-skinned people | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| bush | Shrub or clump of shrubs | Pubic hair; rural person; to ambush | 🟢 Gain | 🟢 Gain | ⚪ Stable |
| cad | Dishonest man; scoundrel | “Computer Aided Design”; “Ctrl-Alt-Del”; “Cadillac” | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| cheese | Food from curdled milk | Money; marijuana; fake smile; bodily fluids; nonsense | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| cheesy | Tasting of cheese | Corny; cheap or fake; marijuana | 🟢 Gain | ⚪ Stable | ⚪ Stable |
| chronic | Long-lasting (medical) | High-quality cannabis; excellent | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| chump | Foolish or gullible person | Common worker; unsophisticated person | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| climber | Person or plant that climbs | Social climber; cat burglar | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| clip | Fastener; short cut | Rob; kill; drug bundle | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| cooker | Cooking appliance | Meth manufacturer; sexy person; “high” | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| cook | To prepare food | To make meth; to falsify; to kill; to perform exceptionally | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| cool | Slightly cold; calm | Fashionable; trustworthy; “to die” | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| cooler | Container for cooling food | Prison cell; drug-laced cigarette | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| coon | Raccoon | Racial slur; sly person; goth makeup | 🔴 Loss | ⚪ Stable | ⚪ Stable |
| crush | To press or squeeze | Romantic attraction; soft drink; obsession | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| cucumber | Vegetable | Penis | 🟢 Gain | 🟢 Gain | ⚪ Stable |
| dap | Fist-bump greeting | Respect; acknowledgment; stylish | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| dew | Water droplets | Sexual fluid; marijuana; Mountain Dew | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| dinosaur | Prehistoric reptile | Outdated person; heroin slang | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| dip | Lower or submerge | To leave; pickpocket; drug user; stylish | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| douche | Cleaning product | Foolish or arrogant person | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| drag | To pull; theatrical clothing | Smoking; drag performance; boring event; insult | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| dude | Man; person | Friendly greeting; “cool person”; stoner slang | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| epic | Heroic poem | Remarkable; extreme; amazing | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| fan | Device for air movement | Pickpocket; to calm down | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| femme | Woman | Feminine partner in LGBTQ+ context | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| fig | Fruit | Genitals; slur; counterfeit coin; pickpocket | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| flutter | Quick wing movement | Gamble; sexual adventure; gay man | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| foam | Froth; bubbles | Beer; gamer slang for anger | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| frog | Amphibian | French person; condom; to cheat | 🟢 Gain | 🟢 Gain | ⚪ Stable |
| gay | Cheerful; bright | Homosexual identity; flamboyant; stupid (slang) | 🔴 Loss | 🟢 Gain | 🟢 Gain |
| ghost | Spirit | Ignore someone; vanish; murder | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| gosh | Euphemism for “God” | Mild exclamation of surprise | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| germ | Microorganism | Idea origin; insult; cigarette | 🟢 Gain | ⚪ Stable | ⚪ Stable |
| mammy | Mother figure | Racial stereotype; “abundance” slang | 🔴 Loss | 🟢 Gain | 🟢 Gain |
| moose | Animal | Large person; unattractive woman; close friend | 🟢 Gain | 🟢 Gain | ⚪ Stable |
| mug | Cup; face | Fool; victim; face; to kiss | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| penguin | Bird | Soulmate; nun; LSD drug | 🟢 Gain | 🟢 Gain | ⚪ Stable |
| player | Participant in a game | Womanizer; manipulator; dealer | 🟢 Gain | 🟢 Gain | ⚪ Stable |
| posse | Legal group | Crew; gang; friends | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| psych | Psychology | To trick; to prepare mentally; to intimidate | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| ratchet | Tool mechanism | Unrefined woman; wild; pistol | 🟢 Gain | 🟢 Gain | 🟢 Gain |
| salty | Tasting of salt | Angry; bitter; crude | ⚪ Stable | ⚪ Stable | ⚪ Stable |
| scum | Layer of dirt | Worthless person; semen | ⚪ Stable | ⚪ Stable | ⚪ Stable |

---

### 📄 Citation
If you use this dataset, please cite:  


