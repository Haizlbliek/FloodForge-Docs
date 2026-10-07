# Knowledge Book

## Room visual merge
When rooms are close to each other,
tiles may overlap and cover sections that should be visible.
Toggling  *merge*  on the overlapping rooms will draw their solid tiles behind everything else,
fixing the overlap.

## Canon vs Dev positioning
Rain World has the ability to have two different position types:  *Canon*  and  *Dev.*
- **Canon**: Shown on the in-game map. Uses all three layers
so rooms in different layers can overlap.
- **Dev**: Used in tools like Cornifer and the dev map. Rooms are spread out to avoid overlap.

You can switch between modes with the `Canon`/`Dev` button.
Rooms are positioned according to the selected mode.
Hold ALT to display the room's other position, shown at half transparency.
Moving a room affects only the active mode.
In order to move both positions, hold ALT while dragging.

## Default vs Path connections
Floodforge can visualise connections in two ways: *Default* and *Path.*
- **Default**: Same as the in-game map. Connections go from the
entrance of one shortcut to the entrance of the other.
- **Path**: Connections start at the end of a shortcut's path, 
usually a little distance from the shortcut's entrance.
In a way this better visualises the 'actual' geometry of a connection.

- This does not affect the in-game map.
It only serves to reduce visual clutter while in Floodforge.

## Adding Reference images
When making a region, you may have made a rough (or very polished) plan.
FloodForge allows you to use such an image as reference.
To add a new reference image:

1. `Edit` -> `Add Reference`
2. Navigate to the relevant image
3. `Open`

The reference image will behave similarly to rooms, but is *not* exported,
and does not affect the in-game map.
To resize the image, right click it and drag the `Scale` slider.
To delete the image, similarly to a room, select or hover over it and press `X`.

## Adding custom mods
Some mods add creatures or timelines to the game, these will show up as `?` in FloodForge until you add them.
To show the proper icons and be able to add the creatures and timelines to new rooms:

1. Add a folder inside `assets/mods` with the mod name (e.g. `assets/mods/silly_mod`)
2. Inside add a `creatures` and `timelines` directory.
3. Inside the `assets/mods/<yourmod>/creatures`, put a .png image for every creature you want to add.
- Make sure the .png name matches your creature id! (e.g. `GreenLizard.png` for GreenLizard)
4. Inside the `assets/mods/<yourmod>/timlines`, put a .png image for every timeline you want to add.
- Make sure the .png name matches your slugcat id! (e.g. `MyCustomScug.png` for MyCustomScug)
- This is directly equivalent to the Slugbase id field.
5. In `assets/mods.txt`, add a line with your directory name.

> **Side note:**
> Sometimes, mods add custom "parsings" for creature names, allowing alternate
> IDs to be used. An example of this are most Lizards; The Green Lizard can be put
> in the world file with either `GreenLizard` OR `Green`.
> 
> Adding your own is pretty simple,
> In `assets/mods/<yourmod>/creatures/parse.txt` add a line with the format:
> `Abbreviated Name>ActualID`
> 
> You can add as many as you like!