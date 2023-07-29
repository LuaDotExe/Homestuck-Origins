# Homestuck Origins
Homestuck Origins is a new community project in which we utilize Origins (Forge), Apugli, and Origins Extra Keybinds to recreate the mechanisms of Homestuck's Title system (commonly referred to as a "Classpect"). This data pack also relies on the Minestuck mod for progression, and is designed to be used alongside it.

In Homestuck, characters are given a mythological role that is referred to as their "Title". A Title is made up of a Class and an Aspect, of which there are both 12. An "Aspect" is essentially an element of reality, and your "Class" dictates how you interface with it. A few of the well-known Titles in Homestuck include Heir of Breath (one who inherits freedom/the wind), Knight of Time (one who weaponizes time itself), and Prince of Hope (one who destroys your last hope).
## CLASSES EXPLAINED
Classes are the first component of a Title. In the project, they will be stored under `data/homestuck/origins/class`. On a technical level, it doesn't do anything on its own-- but on a thematic level, it describes how the player interfaces with their Aspect. The guidelines for this are below:
- **Bard:** One who destroys with their Aspect.
- **Heir:** One who inherits their Aspect. (Probably make this a generic jack-of-all-trades Class)
- **Knight:** One who protects their Aspect. (Probably more leaning on the tank side)
- **Mage:** One who gains knowledge of their Aspect.
- **Maid:** One who gives their Aspect.
- **Page:** One who slowly grows to embody their Aspect. (Difficult early game, spicy rewards; generally radiating their Aspect)
- **Prince:** One who destroys their Aspect.
- **Rogue:** One who steals/steals from their Aspect for others.
- **Seer:** One who divines information from their Aspect.
- **Sylph:** One who heals their Aspect.
- **Thief:** One who steals/steals from their Aspect for themselves.
- **Witch:** One who manipulates their Aspect.
## ASPECTS EXPLAINED
Aspects are the second component of a Title. In the project, they will be stored under `data/homestuck/origins/aspect`. On a technical level, it doesn't do anything on its own-- but on a thematic level, an Aspect is one of the 12 fundamental forces of the universe. They are as follows:
- **Blood:** Bonds, relationships, and unity. "Blood brothers". Opposite to Breath.
- **Breath:** Freedom and the literal wind ("The Breeze"). Opposite to Blood.
- **Doom:** Death, the end of cycles, rules/restrictions, and fate. Opposite to Life.
- **Heart:** The self, the soul, emotion, motive, and intuition. Opposite to Mind.
- **Hope:** Ideals, faith, belief, and literal hope. Opposite to Rage.
- **Life:** Growth, nature, and life itself. Opposite to Doom.
- **Light:** Fortune, knowledge, and literal light. Opposite to Void.
- **Mind:** Logic, rationale, thought, and decisions. Opposite to Heart.
- **Rage:** Chaos, negative emotions, truth, and brute strength. Opposite to Hope.
- **Space:** Self-explanatory. Opposite to Time.
- **Time:** Self-explanatory. Opposite to Space.
- **Void:** Secrets, obscuration, and the very absence of things. Opposite to Light.

## GENERAL FILE STRUCTURE

The `data/origins` folder will contain sub-folders `aspect`, `class`, and `title`. For your purposes, `title` will be the only one that you will actually meddle with, and is to be considered the actual functional origin.

Your Title should point to powers within a specific sub-folder. The `data/powers` folder will contain subfolders named after each Aspect, which will each contain sub-folders named after each Class.

There are certain naming conventions to follow. If you, for example, had a Power named `steal_fortune.json` for the Thief of Light, the origin would be `data/homestuck/origins/title/light_thief.json`, while the power would be `data/homestuck/powers/light/thief/steal_fortune.json`