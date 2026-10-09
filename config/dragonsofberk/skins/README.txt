Dragons of Berk — your own dragon skins
=======================================

1. Put a PNG in the folder named after the dragon, next to this file.

       night_fury/aurora.png

   Paint over the skin the mod already ships if you want a starting point;
   the image must have the same size and layout, or it will look scrambled.

2. Open  config/dragonsofberk-skins.toml  and add one line under that species:

       night_fury = ["1000 | 40 | aurora"]

       1000  the skin's number. Pick anything from 1000 up, and use a different
             one for each skin. IMPORTANT: once dragons are wearing it, do not
             change it - they would all change appearance.
       40    how common it is, 0 to 100. 100 is as common as a normal skin,
             0 means it never turns up on its own.
             Careful: a rarer skin also takes MORE FEEDS to tame, exactly like
             the mod's own rare skins.
       aurora  the file name, without .png

3. Just save the file - the new line applies right away, even to players already
   in the world. If this is the FIRST time you're adding a skin to this species,
   run  /reload  (or restart) once too, so the game notices the new PNG.

On a server, the SERVER's toml is the one that counts, and it is sent to players
when they join, and again whenever it changes. A player who does not have your
PNG just sees the dragon's normal skin - nothing breaks for them.

EXTRA TEXTURES (optional)
------------------------
Two dragons draw a second texture on top of the body:

  Deadly Nadder   the wing membranes    <name>_membranes.png
  Terrible Terror the sleeping pose      <name>_sleeping.png

Drop that file next to your body PNG (same folder, same <name>) and it is used
automatically. Leave it out and the dragon keeps the mod's default for that part -
a Nadder shows the standard membranes, a sleeping Terror shows your awake skin.
