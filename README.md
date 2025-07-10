# Mortal Kombat Mythologies: Sub-Zero - Randomizer
## Intro

Rediscover Sub-Zero’s journey like never before!

This is a mod that completely shuffles the item distribution in Mortal Kombat Mythologies: Sub-Zero, delivering a fresh and challenging experience for both veterans and newcomers. Items, keys, and even power-ups are now placed at random.

In addition, the randomizer grants immediate access to all levels from the start, allowing for a non-linear playthrough. The experience requirements to complete the game have also been adjusted, making progression more flexible and suited to the randomized structure.


### Key Features:

- Randomized placement of all in-game items
- Full access to every level from the beginning
- Overlay UI for key items tracking
- Item management modified to expand capacity
- Seed viewing and input for replaying same runs


The mod is provided AS-IS and in no way, shape and form I commit to maintain this and/or fix whatever bugs are found. You're welcome to report them, and/or fix them on your own, tho!


---

### Instructions for playing

In order to play, you need the latest version of BizHawk emulator, and your own legally obtained rom (z64 format) of the N64 version of the game. And also, you need to set the video resolution to 640 x 480 for the UI to correctly display.

1. Open BizHawk emulator
2. Load your rom
3. In the top menu select N64 > Plugins
4. Set Video Resolution to 640 x 480 and save settings
5. In the top menu select Tools > Lua Console
6. Load the provided script

If everything went as expected, the lua console output shouldn't display any errors, and should also display a few messages of the modules loaded.

---

## Seeds

In order to view current seed, you can do so on the lua console, and/or in the main menu going to Options > Seed. You can freely input any seed you want to play here too. 

---

## Gameplay

### Levels
In order to start, from the main menu, just set the cursor to "Start" and press the A button. That should bring the level select menu. This menu is actually a left-out debug option that was just unlocked via gameshark code, and so you must be warned that selecting either "Unused", "Fire god room" or "Test Characters" will softlock the run and everything would need to be reloaded.

As levels may not be completeable (because its required key could be somewhere else), you may freely hit pause > exit, in order to get back to the main menu, to then go to another level. That's the main gameplay loop.

### Items
Every single pickup item has been internally shuffled, however the icon of the item itself displayed on the level remains the same (we can call this a visual bug). Required keys to finish a given level could be located somewhere else in the game. Also new to the game, is that experience is not gained anymore, and new powers are found as items. A few "herbs" items have been replaced in the pool in order to have said power-ups 'itemified'. However, power-up progression stays the same. Whenever you find a power-up item, you'll get the next power in the vanilla progression. (eg. None > Ice > Slide, etc).

### UI
You can see all found / total checks by opening the item menu. It should be visible in the lower-middle portion of the screen. Also in here, you can see at the top what keys you have for each level. Each level has its own color code (grey is for the keys yet to be found). And the "Powers required" is the amount of power-ups you need in order to fight Quan-Chi after finishing the Fortress level (otherwise it will take you to a 'Game Over' screen.
In this screen you can also go to a different "page" of items by pressing the left/right keys, this is to overcome the need of having more than 10 items. However, this workaround has its own caveats, as a few extra limitations had to be implemented in order to account for bugs:
- Empty spaces are filled with a dummy "-----" item now, and although selectable, they do nothing when used
- Key items from other levels are displayed as "Key Item" instead of "Key" to prevent misuse
- After using an item, the pagination is locked until the menu is closed and open again

---

There might be a few visual bugs here and there from time to time. So far, those have been proven to be minor, anyway.

In order to finish the game, one must find the 3 Crystals (Fortress Key items), have at least the required amount of power-ups, and then go to the Fortress level, enter all 3 Crystals, Fight Quan-Chi, and finally fight Shinnok.