# Phylogeny: Consumption Core

> **The Apex Protocol:** Adapt. Survive. Pass the Torch.

## 🧬 Project Overview
**Phylogeny: Consumption Core** is a **Bio-Punk 3D ARPG** that fuses the interconnected exploration of a Metroidvania with the high-stakes progression of a Rogue-lite.

You play as the **C0RE**—an adaptive nanite cluster—capable of constructing and piloting biological bodies. Your goal is to refine your lineage by hunting dangerous organisms, assimilating their biology, and integrating technology to survive a hostile, evolving planet.

---

## 🎮 The "Visceral Evolution" Loop

The game follows a strict cycle of adaptation and inheritance. There is no safe extraction; you play until you die.

1.  **Create:** Spawn at the Hub as a base organism.
2.  **Explore:** Traverse the fixed Overworld and delve into procedural "Nests."
3.  **Gather:** Defeat enemies to loot **Raw** biological parts and tech scrap.
4.  **The Choice:**
    * **Subsume:** Destroy the item for immediate Biomass (HP) and Crafting Reagents.
    * **Equip:** Graft the item to your body for Power. **(Item becomes Bound/Integrated).**
    * **Hoard:** Carry the Raw item in your Bio-Sac (Inventory).
5.  **Bank:** Return to the C0RE to convert **Raw** items into Genetic Data (XP) based on your **Resonance**.
6.  **Die:** Fall in battle. Your body (Husk) remains where it fell.
7.  **Recover:** Respawn as the next generation. Travel to your ancestor's Husk to reclaim the Lineage.

---

## ⚙️ Key Mechanics

### 1. The Golden Rule of Nanite Adaptation
The distinction between **Equipping** and **Subsuming** is defined by *how* the Nanites interact with matter.
* **Raw State (Inventory):** Inert. Can be traded at the Hub for XP or used in Crafting.
* **Integrated State (Equipped):** The Nanites have physically restructured the item to fit the Host. It provides stats/skills, but **it can no longer be Subsumed for value.** It is bound to the current run.

### 2. Resonance & The Economy
* **Resonance:** A dynamic multiplier that fills as you kill enemies, explore new zones, and survive.
    * *Low Resonance:* The C0RE processes data inefficiently (Low XP payout).
    * *High Resonance:* The C0RE maximizes data extraction (High XP payout + Bonus Yields).
* **The Hub Loop:** You can return to the Hub anytime, but "Safe Grinding" yields almost nothing. To make real progress, you must build high Resonance in the field before returning to cash in.

### 3. The Tri-Layer Paper Doll
Every body slot (Head, Torso, Arms, Legs) has three independent layers:
* **Layer A: Anatomy (The Part):** Biological limbs/organs. Determines **Movement & Abilities**. (e.g., *Raptor Legs* = Sprint).
* **Layer B: Attire (The Cloth):** Soft gear/utility. Determines **Resistances & Passives**. (e.g., *Thermal Vest* = Cold Resist).
* **Layer C: Plating (The Armor):** Hard defense. Determines **Mitigation & Triggers**. (e.g., *Spiked Shell* = Thorns Dmg).

### 4. Crafting: Synthesis & Incubation
Crafting is split by location and risk.
* **Field Synthesis (The "Dirty" Craft):**
    * *Location:* Anywhere.
    * *Result:* Combines two Raw items into one **Integrated** item.
    * *Risk:* High chance of Negative Mutations.
    * *Use Case:* Emergency survival.
* **Hub Incubation (The "Clean" Craft):**
    * *Location:* C0RE Hub.
    * *Result:* Combines two Raw items into one **Raw** item.
    * *Risk:* None. High chance of Synergy Bonuses.
    * *Use Case:* Preparing a build for the next run.

---

## 💀 Death & Lineage

* **The Husk:** Stores your Equipped Gear, Inventory, and current Resonance Snapshot.
* **Decay:** Time reduces the integrity of the Husk. Speed is required to recover full value.
* **Hardcore Options:**
    * *Standard:* Death resets Resonance/XP if Husk is lost.
    * *Dead-is-Dead:* Failing to recover the Husk causes **Lineage Collapse** (Save Wipe).

---

## 🌍 World Structure

* **Macro-World (Metroidvania):** Handcrafted, persistent map. Areas are gated by Anatomical Traits (e.g., need *Gills* for the Sunken Zone).
* **Micro-Nests (Rogue-lite):** Procedural dungeons. Layouts persist for the life of the current character but re-roll upon Death/Rebirth.

---

## 📝 Roadmap: Phase 1

- [ ] **Repo Init:** Set up `phylogeny-consumption-core`.
- [ ] **Core Controller:** Implement the `NaniteHost` (Player) vs. `Chassis` (Body) separation.
- [ ] **Loot Logic:** Create `ItemData` with states: `Raw` vs `Integrated`.
- [ ] **Resonance System:** Implement the "Kill-to-Multiplier" logic.
- [ ] **Inventory:** Build the Grid (Bio-Sac) and the Tri-Layer Paper Doll backend.
- [ ] **Death Loop:** Spawn Husk prefab -> Save Data to Husk -> Clear Player Data.
