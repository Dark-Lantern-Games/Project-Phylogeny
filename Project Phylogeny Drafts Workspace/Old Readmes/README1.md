# Phylogeny: Consumption Core

> **C0RE Protocol:** Create. Explore. Consume. Evolve. Die. Repeat.

## 🧬 Project Overview
**Phylogeny: Consumption Core** is a **Bio-Punk 3D ARPG** that blends that blends the exploration of a Metroidvania with the high-stakes progression of a Rogue-like aside deep itemization and customization options.

You are the **C0RE** — the Central Operational Research Engine — an adaptive nanite cluster capable of constructing and directly piloting biological bodies. Your goal is to refine and secure your lineage by hunting dangerous organisms and mechanical constructs, then assimilating their biological makeup and technical capabilities to survive a hostile, evolving planet.

---

## 🎮 The "Visceral Evolution" Core Gameplay Loop

The game follows a strict cycle of adaptation and inheritance. There is no safety.

1. **Create:**  The player spawns their character as a base organism — **The Null Strain**
2. **Explore:** Traverse the fixed Overworld and delve into procedural "Nests"
3. **Gather:** Defeat enemies and loot their corpses for **Raw** biological and mechanical parts, clothing, armor, and scraps
4. **The Choice:**
   * **Subsume:** Absorb the loot for immediate but reduced benefits and crafting reagents
   * **Equip:** Graft items to your body for immediate but reduced stat bonuses. **(Item is integrated, cannot be removed/subsumed)**
   * **Hoard:** Carry the item in your Bio-Sac (inventory).
5.**Bank:** Return to C0RE to convert the **Raw** items into Genetic Data or Technological Components based on your **Resonance**.
6. **Die:** Falling in battle is an inevitability. The world  is violent and unforgiving. You will perish. Your shell remains.
7. **Recover:** A new C0RE body is created — you respawn as the next generation. Travel to your ancestral Husk and reclaim your Lineage.

--- 

## ⚙️ Key Mechanics

### 1. The Golden Rule of Nanite Adaptation
The distinction between **Equipping** and **Subsuming** is defined by *how* the character's Nanites interact with matter:
* **Raw State (Inventory):** Inert. Can be turned in at C0RE for Genetic Points (organic) or used in crafting (mechanical/technical)
* **Integrated State (Equipped):** The Nanites have physically restructured the item to fit the Host. It provides stats or skills, but **it can no longer be Subsumed.** The equipment is now bound to the current husk (and therefore, the current generation).

### 2. Resonance & The Economy
* **Resonance:** A dynamic multiplier that fills as you kill enemies, explore new zones, and survive.
   * *Low Resonance:* The C0RE processes the data inefficiently — more (xp/kills/etc) needed
   * *High Resonance:* The C0RE maximizes data extraction — increased XP, yields, etc.
* **The Hub Loop:** You can return to the C0RE at any time, but "Safe Grinding" yields virtually nothing. To make real progress, you must build up Resonance before turning in your spoils.

### 3. The Tri-Layer Paper Doll System ("Evolootion")
In *Phylogeny*, every body slot (head, torso, arms, legs, fingers, etc) has three independent layers:
* **Layer A: Anatomy (The Part):** Biological limbs, organs, etc. **Movement & Abilities**. (t.g., *Raptor Legs* = Sprint).
* **Layer B: Attire (The Clothing):** Soft gear and utility. Shirts, pants, & undergarments, but also belts, bags, & jewelry. **Resistanaces & Passives**. (e.g., *Thermal Vest* = Cold Resist).
* **Layer C: Plating (The Armor):** Hard defense. helmets, boots, torso, etc. **Mitigation & Triggers**. (e.g., *Spiked Shell* = Thorns Damage).
**Grafting:** Loot consists of body parts such as severed limbs and internal organs, or tech scrap. Attaching a "Raptor Leg" grants movement speed and a claw attack.

### 4. Crafting: Synthesis & 

### 2. The Cycle of Inheritance ("Geneticist's Gambit")
You are a lineage, not a single hero. Death is a core mechanic.
* **The Loop:** Spawn -> Explore -> Die -> Respawn as Next Gen.
* **Corpse Retrieval:** You must trek back to your ancestor's corpse to retrieve it.
* **Consumption:** "Eating" the previous generation banks their "Genetic Experience" into the permanent **Phylogeny Web** (passive skill tree).
* **Decay:** Taking too long to retrieve the corpse results in "Rot," reducing the Biomass payout.
* **Permadeath**: Dying before corpse retrieval results in total lineage breakdown

### 3. Bio-Mech Synthesis
Bridge the gap between nature and machine.
* **Mutation:** Consume organic parts for **Biomass** (HP/Regen).
* **Augmentation:** Consume mechanical parts for **Scrap** (Energy/Shields).
* **Synthesis:** Fuse items to create unique hybrids (e.g., *Chitinous Shell* + *Reactive Plating* = *Ablative Carapace*).

### 4. World Structure
* **Macro-World (Metroidvania):** A fixed, handcrafted world layout. Traversal requires specific body grafts (e.g., Wings for verticality, Gills for underwater).
* **Micro-Nests (Roguelite):** Procedural sub-levels (dungeons) that shift layout and enemy density with every new generation.

---

## 🛠️ Technical Pillars

* **Genre:** ARPG / Metroidvania / Roguelite
* **Perspective:** Side-scrolling or Isometric (TBD)
* **Key Systems:**
    * Procedural Item Generation (Affixes/Suffixes)
    * Modular Character Controller (Handling variable limb counts/types)
    * Persistent Data Storage (The Phylogeny Web)

---

## 📝 Roadmap / Todo

### Phase 1: The Proto-Organism
- [ ] Set up project repo & environment.
- [ ] Create basic "Core" movement controller.
- [ ] Implement "Paper Doll" data structure (slots for limbs).
- [ ] Prototype basic "Grafting" (swapping a sprite/mesh on the player).

### Phase 2: The Hunter
- [ ] Implement Enemy AI and "Loot Dropping" (dropping body parts).
- [ ] Create the "Consumption" interaction (convert item to currency/xp).
- [ ] Build the first "Nest" (procedural level generation).

### Phase 3: The Lineage
- [ ] Implement Death & Respawn loop.
- [ ] Create the "Corpse" persistent object mechanics.
- [ ] Build the basic **Phylogeny Web** UI.

---

## 📂 Directory Structure (Proposed)
```text
/src
  /Systems
    /Evolution      # Logic for mutation and stats
    /Loot           # Item generation and affix logic
    /WorldGen       # Procedural nest generation
  /Entities
    /Player         # The Core and modular body parts
    /Enemies        # Mobs and Bosses
  /Data
    /Genetics       # Skill tree definitions
