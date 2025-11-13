# 🧠 BD-LSC: Bi-Directional Lexical Semantic Change  
### A Benchmark Dataset for Tracking Sense Gain, Loss, and Stability in Slang and Standard English

---

## 🔍 Overview

BD-LSC (Bi-Directional Lexical Semantic Change) is the first benchmark dataset designed to detect and analyze bi-directional changes in word meaning, capturing how lexical senses are gained, lost, or remain stable across slang and standard English from the 1980s to the 2020s.

Unlike traditional binary semantic change datasets (e.g., SemEval-2020 or TempoWiC), BD-LSC introduces multi-label temporal annotations across three time periods and integrates both formal corpora (COHA/CCOHA) and informal data (Twitter), enabling a unified view of language evolution across registers.

---

## 🧱 Dataset Composition

| Period | Years | Source | Description |
|:------:|:------|:--------|:-------------|
| T1 | 1980–1999 | CCOHA / COHA | Late 20th-century formal written English |
| T2 | 2000–2009 | COHA | Early 21st-century transitional English |
| T3 | 2010–2020 | Twitter | Contemporary slang and social media language |

### 📚 Target words Sources
- Standard English: COHA, CCOHA, Oxford English Dictionary (OED)  
- Slang: SlangSD, Green’s Dictionary of Slang, Urban Dictionary, Online Slang Dictionary  
- Annotation Quality: 3 expert annotators  
  - Cohen’s κ = 0.92 (T1) / 0.89 (T2) / 0.86 (T3)  

Each target word is labeled for Sense Gain (SG), Sense Loss (SL), and No Change (NC) between periods T1→T2, T2→T3, and T1→T3.

---

## 💬 Target Words and Example Entries

The BD-LSC dataset includes 79 target words (8,000+ annotated senses), covering both slang and standard English.


| Word | No. of Senses | Example Standard Meanings | Example Slang Meanings | T1–T2 Label | T1–T3 Label | T2–T3 Label | Change Type Example |
|:------|:--------------:|:---------------------------|:--------------------------|:-------------|:-------------|:-------------|:--------------------|
| abc | 3 | Alphabet sequence; basic knowledge | Beginner-level; easy as ABC | ⚪ No Change | 🟢 Sense Gain | 🟢 Sense Gain | New informal usage appears online |
| atm | 4 | Cash dispenser; banking terminal | “At the moment” (text slang) | 🔴 Sense Loss (technical narrowing) | 🟢 Sense Gain | 🟢 Sense Gain | Acronym gains new digital sense |
| bam | 6 | Sudden impact; loud sound | Expression of excitement (“Bam!”) | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | Added expressive interjection |
| battery | 5 | Electrical cell; group of artillery | Phone power supply; violent assault | ⚪ No Change | 🟢 Sense Gain | 🟢 Sense Gain | Expanded to tech and legal slang |
| bot | 7 | Robot; automated machine | Automated social media account; fake persona | ⚪ No Change | 🟢 Sense Gain | 🟢 Sense Gain | Digital sense added in T3 |
| bouncer | 5 | Doorman; security guard | None | 🔴 Sense Loss | 🔴 Sense Loss | ⚪ No Change | Occupational term declines |
| bush | 7 | Shrub; rural area | None | 🔴 Sense Loss | 🔴 Sense Loss | ⚪ No Change | Cultural reference fades |
| cheese | 8 | Dairy product; food | Money (“cheddar”); fake smile (“say cheese”) | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | New slang meanings arise |
| cheesy | 8 | Tasting of cheese; cheap quality | Corny, sentimental, exaggerated | 🟢 Sense Gain | ⚪ No Change | ⚪ No Change | Stable slang since early 2000s |
| chronic | 5 | Long-lasting (medical) | High-quality cannabis | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | Cannabis sense appears, medical sense retained |
| chump | 4 | Foolish person | None | 🔴 Sense Loss | 🔴 Sense Loss | ⚪ No Change | Obsolete slang disappears |
| cool | 6 | Cold; calm, composed | Stylish, good, excellent | ⚪ No Change | ⚪ No Change | ⚪ No Change | Meaning stable across periods |
| coon | 5 | Raccoon; old racial slur | None (declining use) | 🔴 Sense Loss | ⚪ No Change | 🟢 Sense Gain | Old slur declines; neutral sense persists |
| crush | 8 | Press or squeeze; romantic infatuation | Online obsession; fan fixation | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | Expands to digital/celebrity contexts |
| douche | 3 | Medical cleaning device | Insult; foolish person | 🟢 Sense Gain | ⚪ No Change | ⚪ No Change | Maintains slang insult sense |
| drag | 11 | Pull or draw with effort | Boring situation; drag performance | 🔴 Sense Loss | 🟢 Sense Gain | 🟢 Sense Gain | Loses literal use, gains cultural sense |
| fan | 5 | Device for air movement; admirer | Sports or media enthusiast | 🔴 Sense Loss | 🔴 Sense Loss | ⚪ No Change | Physical meaning declines |
| femme | 3 | Woman; feminine identity | LGBTQ+ identity marker | 🔴 Sense Loss | ⚪ No Change | 🟢 Sense Gain | Older gendered sense redefined |
| frog | 7 | Amphibian | None | 🔴 Sense Loss | 🔴 Sense Loss | ⚪ No Change | Used less in slang contexts |
| gay | 6 | Cheerful, bright; carefree | Homosexual identity; vibrant, flamboyant | 🔴 Sense Loss | 🟢 Sense Gain | 🟢 Sense Gain | Semantic shift from happy → identity |
| germ | 6 | Microbe; seed origin | Idea origin (“germ of an idea”) | 🟢 Sense Gain | ⚪ No Change | ⚪ No Change | Abstract sense remains stable |
| ghost | 9 | Spirit or apparition | Ignore someone; vanish online; fake account | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | Modern slang expands widely |
| gosh | 2 | Mild oath or exclamation | None | ⚪ No Change | ⚪ No Change | ⚪ No Change | Stable interjection |
| mammy | 4 | Motherly figure; nanny | Abundance; affectionate reference | 🔴 Sense Loss | 🟢 Sense Gain | 🟢 Sense Gain | Cultural sense reinterpreted |
| moose | 7 | Large animal | None | ⚪ No Change | ⚪ No Change | ⚪ No Change | No significant change |
| mug | 11 | Cup; face; rob or attack | Photograph; to pose; to make faces | 🟢 Sense Gain | ⚪ No Change | 🟢 Sense Gain | Adds performative sense |
| penguin | 5 | Bird; symbol for tuxedo | Computer OS mascot (Linux Penguin) | 🟢 Sense Gain | 🟢 Sense Gain | ⚪ No Change | Tech meaning appears |
| player | 5 | Participant in a game | Flirtatious person; manipulator | 🟢 Sense Gain | 🟢 Sense Gain | ⚪ No Change | Romantic/urban slang appears |
| posse | 6 | Legal enforcement group | Group of friends or crew | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | Meaning broadened socially |
| psych | 8 | Relating to mind; psychology | To fake out; to prepare mentally | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | Informal sense added |
| ratchet | 5 | Tool with gears | Loud, brash, or low-class (slang) | 🟢 Sense Gain | 🟢 Sense Gain | 🟢 Sense Gain | Negative slang added |
| salty | 6 | Tasting of salt | Bitter, annoyed, resentful | ⚪ No Change | ⚪ No Change | ⚪ No Change | Consistent slang sense |
| scum | 3 | Dirt or impurity; unpleasant person | Low-status group; insult | ⚪ No Change | ⚪ No Change | ⚪ No Change | Stable derogatory term |
| mammy | 4 | Mother/nanny figure | Affectionate term or abundance slang | 🔴 Sense Loss | 🟢 Sense Gain | 🟢 Sense Gain | Retains cultural nuance |
| cucumber | 3 | Vegetable | None | 🟢 Sense Gain | ⚪ No Change | ⚪ No Change | Phrase “cool as cucumber” persists |
| frog | 7 | Amphibian | None | 🔴 Sense Loss | ⚪ No Change | ⚪ No Change | Literal sense retained only |
| bouncer | 5 | Security guard; doorman | None | 🔴 Sense Loss | 🔴 Sense Loss | ⚪ No Change | Occupational term declines |
| coon | 5 | Raccoon; slur | None | 🔴 Sense Loss | ⚪ No Change | ⚪ No Change | Offensive use fades |
| germ | 6 | Microbe | Idea origin | 🟢 Sense Gain | ⚪ No Change | ⚪ No Change | Abstract meaning emerges |
| bush | 7 | Shrub; rural area | None | 🔴 Sense Loss | ⚪ No Change | ⚪ No Change | Old rural sense diminishes |


🗂️ Full dataset available in `/data/bd-lsc_full.csv`.

---

## 📘 Annotation Schema

| Word | Sense ID | Sense Description | T1 | T2 | T3 |
|------|-----------|------------------|----|----|----|
| fire | 1 | Combustion / flames | ✅ | ✅ | ✅ |
| fire | 2 | Slang: “cool”, “excellent” | ❌ | ✅ | ✅ |
| fire | 3 | To dismiss from a job | ✅ | ✅ | ✅ |

Interpretation:  
✅ = sense present in that period  
❌ = sense absent  

Label rules:
- Sense appears → Sense Gain (SG)  
- Sense disappears → Sense Loss (SL)  
- Sense persists → No Change (NC)  

---

## 🧩 Dataset Creation Pipeline

1. Word selection: Overlap of SlangSD (48k entries) and COHA (169k lemmas).  
2. Filtering criteria:  
   - Appears ≥50 times in at least one period  
   - ≥50% frequency variance  
   - Appears in multiple periods  
   - Verified slang sense (via OED, Green’s, Urban, Online Slang Dictionary)  
3. Annotation: Manual tagging of standard and slang senses per time slice (T1–T3).  
4. Validation: Three annotators, inter-annotator agreement (κ ≈ 0.85–0.92).

---

## 🧬 Research Tasks

### 1️⃣ Lexical Semantic Change Detection (SCD)
Determine whether a word’s sense is added, lost, or stable between periods.

Input: Sense inventories from T1–T3  
Output: {Sense Gain, Sense Loss, No Change}  


## 📊 Baseline Evaluation

| Model | Type | Multi-label Accuracy | Exact Sense Match | Notes |
|--------|------|----------------------|-------------------|--------|
| N-gram ML | Supervised | 0.70 | 0.66 | Good baseline |
| DistilBERT | Supervised | 0.47 | 0.53 | Weak on slang |
| FastText | Supervised | 0.47 | 0.53 | Limited context |
| ALBERT + HDBSCAN | Unsupervised | 0.70 | 0.73 | Robust clustering |
| GPT-4o (few-shot) | LLM | 0.818 | 0.908 | 🏆 Best overall |

Key insight: GPT-4o demonstrates exceptional few-shot generalization for slang-driven semantic change.

---


