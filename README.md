# Mod Design Document: The Silver River (Rise of Saptagram)

**Game Target:** Europa Universalis V **Region:** Bengal / Eastern India **Focus:** Tall Play, Economic Dominance, Cultural Syncretism, "Asian Venice"

## 1. Concept Overview

**"The Silver River"** introduces a new playable **Location-based Tag: the Thikana of Saptagram.**

Unlike the standard territorial conquest loop, this mod leverages EU5's **Dynamic Market** and **Control** systems to build a "Thalassocracy of the Rivers." You play as the **Banik Sabha** (Merchant Council) of Saptagram, aiming to break away from the Tughlaq Delhi Sultanate during their 1337 crisis and establish the world's wealthiest Market Center.

**Core Gameplay Loop:**

1. **Maximize Control:** Maintain 100% Control in the small Bengal Delta core to maximize tax/levy efficiency.
2. **Market Attraction:** Use infrastructure to steal the "Market Center" status from Gaud and Sonargaon.
3. **Foreign Factories:** Use the "Factory" mechanic to build trade posts in Malacca and China without conquering land.

## 2. Starting Situation (1337 AD)

- **Tag:** Saptagram (Thikana of Saptagram).
- **Rank:** County (Start with <100k Primary Culture Pops, upgradeable to Duchy/Kingdom later).
- **Overlord:** Delhi Sultanate (Tughlaq Dynasty).
- **Capital Location:** Saptagram (High Maritime Presence, River Port).
- **Population (Approx):**
  - Total: ~185,000 Pops in capital location.
  - **Burghers:** 25% (Very High - represents the merchant guilds).
  - **Peasants:** 60%.
  - **Clergy:** 10% (Sufis & Brahmins).
  - **Nobles:** 5% (Replaced by 'Merchant Princes' via reform).
- **Goods:** Cotton (Raw Material) and Fabrics (Manufactured Good).

## 3. Unique Mechanics

### A. Government: The Banik Sabha
*   **Type:** Merchant Republic (EU5 Republic mechanics).
*   **Unique Reform:** "Saptagrami Syndicate"
    *   *Effect:* +20% Merchant Capacity, +15% Production Efficiency (Fabrics).
    *   *Drawback:* -10% Maximum Manpower (Reliance on Mercenaries).
    *   *Societal Value:* Pushes towards Plutocracy and Free Subjects.
*   **Cabinet Action:** "Audit the Guilds"
    *   Uses a Cabinet Scholar/Diplomat.
    *   Increases **Burgher Estate Satisfaction** but reduces **Tax Efficiency** temporarily (money stays in the market).

**B. The "Silver Stream" Trade System**

EU5 uses dynamic markets. Saptagram does not start with a Market Center; it belongs to the Gaud Market.

*   **Objective:** Create the Saptagram Market.
*   **Unique Building:** The Grand Ghat
    *   Category: Port/Infrastructure.
    *   *Effect:* +50 Market Attraction in the location. Increases Maritime Presence in adjacent river zones.
    *   *Upgrades:* River Customs House -> Deep Water Dock.
*   **Mechanic:** "The Muslin Charter"
    *   A unique **Privilege** granted to the Burgher Estate.
    *   *Effect:* The Burghers automatically build Weaver Workshops in any owned location with Cotton.
    *   *Bonus:* If Saptagram controls >25% of the Global Trade Volume of "Fine Textiles," gain +10% Prestige Decay reduction.

**C. Cultural Mechanic: The Bengal Renaissance**

*   **Societal Value:** "Syncretism"
    *   Saptagram starts with a unique push towards Tolerance (Societal Value).
    *   "Dharma-Deen" Advance (Age of Discovery): Allows Clergy of both Sunni and Hindu faiths to have >50% Satisfaction simultaneously.
*   **Assimilation:**
    *   Instead of manual conversion, use the "Patronize Arts" Cabinet Action to increase Cultural Assimilation speed in trade ports.

**4. Narrative Content (Journal/Missions)**
# Chapter I: The Tughlaq Default (1337-1350)

*   **Context:** Muhammad bin Tughlaq's token currency experiment is failing.
*   **Objective: "Fiscal Independence"**
    *   **Requirement:** Have a **Positive Budget Balance** for 5 years; Stockpile 500 Gold.
    *   **Action:** "Reject the Copper Token."
    *   **Effect:** Declare Independence. Spawns a 5,000-man **Mercenary Company** (The river guards) for free (Contract paid for 5 years).
*   **Objective: "River Hegemony"**
    *   **Requirement:** Own locations: Saptagram, Hugli, Betor. **Control > 90%** in all.
    *   **Reward:** Advance Unlock: "**Riverine Logistics**" (+15% Movement Speed in River Terrain).

# Chapter II: The Loom of the East (1350-1450)

*   **Objective: "The New Market"**
    *   **Requirement:** Saptagram Location has **Market Attraction > Gaud**.
    *   **Effect:** Saptagram becomes a **Market Center**. Gain permanent +10 Merchant Capacity.
*   **Objective: "Arakanese Elephants"**
    *   **Requirement:** Trade Alliance with Arakan OR occupy Chittagong.
    *   **Reward:** Unlocks "**War Elephants**" as a trainable Levy type (Very high shock, high food upkeep).

# Chapter III: The Emerald Chain (1450+)

*   **Objective: "Factory of the Straits"**
    *   **Requirement:** Build a **Trade Factory** (Diplomatic Interaction) in a location belonging to the **Malacca Market**.
    *   **Reward:** "**Straits Supremacy**" Advance (Galleys gain +20% Combat Ability in Coastal Waters).

## 5. Unique Advances (Tech/Traditions)

In EU5, "National Ideas" are replaced by **Unique Advances** in the tech tree.

### Age of Tradition (Starting Advances):

1.  Saraswati's Blessing: +15% Maritime Presence generation.
2.  Subarnabanik Banking: Interest per Annum -1%.

### Age of Discovery (Unlockable):

1.  Mangalkavya Literature: +0.10 Monthly Stability.
2.  Jagadishpur Gunpowder: Unlocks "Firearm Infantry" regiments 10 years earlier than neighbors.
3.  Deep River Dredging: Construction Cost -10% for Infrastructure/Ports.
# 6. Flavor & Events

## 1. The Siltation of the Saraswati (Disaster/Situation)

*   **Mechanic:** A hidden "Silt" counter increases yearly.
*   **Trigger:** If "Silt" > 50, **Market Attraction** in Saptagram begins to decay.
*   **Resolution A (Historical):** "Found Kolkata." Move capital to the location of Kalikata. Costs Gold, but resets Market Attraction.
*   **Resolution B (Alt-History):** "The Great Dredging." Cost massive amounts of **Wood** and **Gold**. Keep Saptagram as the capital; gain "Eternal Harbor" modifier (+25% Local Defensiveness).

## 2. The Portuguese Arrival (1498+)

*   **Trigger:** European nation with "Caravels" enters the Bay of Bengal.
*   **Interaction:**
    *   **Option A:** "Grant the Farman." Allow them to build a Factory. Gain "Western Arms" (Military Tech boost).
    *   **Option B:** "The River is Ours." War. If won, gain +10 Prestige and +5 Merchant Power in the Cape Market.

# 7. Modding Implementation Details

## 1. Map Edits:

*   Split the Saptagram location to ensure density.
*   Check Vegetation/Topography: Ensure Saptagram is defined as **Farmlands/River** (High pop capacity).

## 2. Files to Mod:

*   common/countries/: Define SAP - Saptagram .
*   common/government_reforms/: Add saptagram_mercantile .
*   common/advances/: Add the unique tech tree nodes.
*   common/buildings/: Add grand_ghat (Special port variant).

## 3. Mercenaries:

*   Define a unique mercenary company "The Bagh-Mari" (Tiger Killers) available only to Saptagram, emphasizing **Light Infantry** (good in Jungle/River).
