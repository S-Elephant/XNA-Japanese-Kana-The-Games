===============================================================================
=                                 General                                     =
===============================================================================
This game can be downloaded for free from:
https://sourceforge.net/projects/japanesekana/

Some resources within this project may have their own license. Check out the
Credits.txt file for more info about the licenses.

"Japanese Kana - The Games" © 2012 Napoleon, is licensed under the Creative
Commons Attribution-ShareAlike license
(http://creativecommons.org/licenses/by-sa/3.0/).

===============================================================================
=                               Installation                                  =
===============================================================================
1. Download the latest version of the game and unzip it.
3. Install the XNA framework from:
   http://www.microsoft.com/en-us/download/details.aspx?id=20914
3. Start the game by launching "Japanese Kana - The Games.exe".

Notes:
- If you run windows XP or an older OS make sure that you have the .NET 4.0
  Framework installed.
- If you run this game from inside virtual machine the screen might go black
  when changing resolutions. Restart the game to fix this.
- This game requires the Windows Media Player to be present in Windows (in case
  you de-installed it this game will crash)
- Needs ~500MB RAM. Why this much? Because it caches all the Japanese
  characters in memory.

===============================================================================
=                              Game explanation                               =
===============================================================================
<<Cars>>
Shoot the car that matches the Romaji shown on top of the screen. If there are
multiple cars with the right answer then any of those will do.

- When the last car with the matching character leaves the screen you lose
  study points and a new Romaji will be shown. It will also briefly show a red
  balloon with the matching Romaji.
- When you shoot the wrong car the matching Romaji for that car will be
  displayed in a red balloon.
- Click on the button in the lower left corner to change the speed setting.

[Left Mouse Button]  = Shoot
[Right Mouse Button] = when hovering over a car it will display it's matching
                       romaji in a white balloon
[Escape]             = Exit to main menu




<<Memory>>
- Just like the original Memory game only here you have to match Romaji cards
  with Kana cards.

[Left Mouse Button]  = Select the card under the mouse
[Directional Keys]   = Change the card selecters position
[Enter]              = Select the card within the selector
[Escape]             = Exit to main menu




<<Runner>>
- Enemies run from the left to the right. Enter their translations before they
  reach the right side of the screen. Always enter the translation for the
  enemy with a yellow/gold box around it's Kana. This is the 'active enemy'.
- Every x seconds you may launch a bomb that will kill all enemies. It costs
  study points depending on the amount of enemies on the screen.
- Use the buttons in the lower left corner to change various settings
	- 'Lightning bolt' = Change spawn speed
	- 'Lightning Bolt & Cow' = Change movement speed
	- 'Bird' = Enable/Disable flyer spawns
	- 'Lock' = (Un)lock the active enemy until it dies or leaves the screen.

[Alphanumeric Input] = Enter translation
[Enter]              = Confirm translation
[Spacebar]           = Launch bomb (if not on cooldown)
[Escape]             = Exit to main menu
[F1]                 = Shows the correct answer at the cost of some SP.


<<Vocabulary>>
- Type the romaji (Rom) translation for the word shown in the center of the
  screen.
- Then type it's english translation.
- Use the button in the lower left corner to switch between 'type'- and
  'image' mode.
- When the image mode is active you may select the picture that matches the
  word shown in the center of the screen instead of typing.

Buttons:
- The button with the image/keyboard changes the mode.
- The button with "Help" written on is the same as pressing [F1]
- The recycle button will put words that you answered incorrect (or not in 1
  try) back into the pool of words for that round until it is correctly
  entered correctly (in 1 try).
- The button with the "a - Z" with the arrow beneath it opens a menu that
  allows the player to set the range of active words for the current
  vocabulary.
- The button with "case" written on it determines whether both the romaji and
  English translation input are case-sensitive (green) or not (red).
- The button with "swap" written on it determines whether the typos like "dgo"
  or "odg" validate against "dog". Does NOT apply to the romaji input.
- The button with "info" written on it determines whether words with the
  "ExtraInfo" element (non-empty) have this info displayed at the end of the
  turn.
- The button with the Hiragana "A" image button determines whether or not the
  romaji translation part is skipped (red). Green = not skipped. Clicking this
  buttin will also reset the current round.
- The button with "space" written on it determines whether spaces are taken
  into acount when validating (green = take into account, red = ignore spaces).

[F1]                 = Show the correct answer at the cost of some SP.
[Left Control]       = Extends the current input with the extender word #1 in
                       the profile (default "masu").
[Right Control]      = Extends the current input with the extender word #2 in
                       the profile (default "masu").
===============================================================================
=                                Feature List                                 =
===============================================================================
- Full HD resolution support.
- Includes the Kana (Hiragana & Katakana including the entire Yoon).
- Supports multiple users (not simultaneously).
- Comes with 3 games.
- Most games can have some of their options changed ingame.
- The Memory game has 4 different AI's and the option to play solo.
- The Vocabulary game has over 10 different adjustable settings.
	
===============================================================================
=                                  XML Info                                   =
===============================================================================
The space character is supported
-- = Choonpu (dash-like character)
.  = dot
DD = Sokuon (small tsu)

Note that the tab-character is not allowed for the vocabulary XML entries. The
spritefonts do not include the tab-character.
         
===============================================================================
=                            Known Bugs & Issues                              =
===============================================================================
Issues:
- Sometimes when switching between resolutions in fullscreen mode a black/blue
  border is shown. Restart the game to fix this, it won't come back unless you
  change resolutions again.

Known Bugs:
- The AI in Memory sometimes picks only one card.
- Sometimes the Vocabulary's image-select-mode will not display the correct
  image. It usually only occurs for the first image after loading a vocabulary
  or switching for the first time to image-select-mode.

===============================================================================
=                                 Changes                                     =
===============================================================================

Version 0.1.2 (05-08-2012):
  - Slightly improved the error information for the vocabulary.
  - The Vocabulary can now handle words with no image(s).
  - Fixed an infinite loop that occured when the Vocabulary XML file contains
    less than 8 images total.
  - The vocabulary now also shows the correct image for the last word in the
    round in typing mode.
  - Switched the " and ' characters.
  - Added the F1 button to the Runner game.
  - Fixed the 'perfect entries' count when the recycling option is on.
  - The Vocabulary Romaji input is no longer case sensitive.
  - The vocabulary now correctly remembers and restores the last used mode for
    the player (this was bugged in version 0.1.1)
  - Added a lot of extra features/buttons to the Vocabulary game.
  - Added button tooltips
  - Added the left- & right control to the Vocabulary.
  - Added 2 new attributes to the Vocabulary translations
  - Added a new project to easily add and maintain the vocabularies XML.
  - Words that were answered incorrectly may no be put in the pool for the next
    round. This way the player can repeat the incorrectly answered words over
	and over again without bothering with entering all the known words.
  - Added file versions to the vocabulary XML files.
  - The XMl documents are now loaded with the "PreserveWhiteSpace" option.
    Space characters in the Romaji Characters don't crash anymore.

Version 0.1.1 (18-07-2012):
  - Added a new game: Vocabulary.
  - Fixed a bug regarding the locations of the answers in Runners.
  - Removed the "di" & "zi" Hiragana glyphs.
  - Fixed a bug that was randomly clearing the in-game controls during gameplay
    Hint: destructors+clearing of lists+garbage collector == stupid.
  - Disabled the Library because it was not finished.

Version 0.1.0 (05-07-2012):
  - First release