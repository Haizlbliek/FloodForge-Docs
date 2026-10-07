# World Editor

Lorem Ipsum

## Controls

Middle click + drag to move camera
Scroll to zoom

Ctrl+Z - Undo
Ctrl+Y - Redo
X - Delete
C - Open creature den
G - Toggle visual merge
W - Toggle warpable through Warp Menu mod
L - Change layer
T - Change tag
S - Change subregion
A - Change attractiveness
H - Toggle visibility
I - Move to back
D - Change conditionals
R - Open room in Droplet
F - Search for room
B - Toggle bat migration blockage
Alt+T - Open Tutorial
Alt+S - Open Splash
Right click - Open reference image settings; Reset popup size


## How to...

### Creating a new region
- `File` -> `New`
- In the popup, type your region acronym
- `Confirm`

### Importing an existing region
- `File` -> `Import`
- Navigate to your `world\_xx.txt` file (`mods/YOUR_MOD/world/xx/world_xx.txt`)
- `Open`

### Adding rooms to a region
*After creating or importing a region*
- `Edit` -> `Add Room`
- Navigate to `mods/YOUR_MOD/world/xx-rooms/XX_A01.txt`
- `Open`

### Connecting rooms
- Find two room exits between two different rooms
- Right click and drag from the first room exit to the second

### Adding creatures to a den
- Choose a den, hover it, and press `C`
- In the popup, select the creature you wish to add
- Click multiple times for multiple of the same type of creature

### Lineages & multiple types of creatures
*After opening a den, the left section controls lineages*
`<` -> Select previous lineage
`x` -> Delete selected lineage
`+` -> Add new lineage
`>` -> Select next lineage
- Creatures in the lineage are vertically placed
- Press the large `+` at the bottom to add a new creature
- Press `...` to edit conditionals (See `Conditionals`)
- Press `x` beside a creature to remove the creature from the lineage

### Conditionals
- Either by pressing `D` while hovering a connection or room,
or by pressing `...` in a den lineage

**Connections and creatures:**
`ALL` -> This is visible to  *all*  slugcats
`ONLY` -> This is  *only*  visible to selected slugcats
`EXCEPT` -> This is visible to all slugcats  *except*  selected ones

**Rooms:**
`DEFAULT` -> This room has  *default*  visiblity
`EXCLUSIVE` -> This room is  *exclusive*  to selected slugcats
`HIDE` -> *Hide*  this room on selected slugcats

**World View**
- Pressing the `Timeline` button in the top bar shows a similar menu.
This decides what conditionals are shown.
`ALL` -> Shows *all* conditionals
`ONLY` -> Shows *only* the conditionals visible to the selected slugcats.
`EXCEPT` -> Shows all conditionals *except* those
limited to `ONLY` the selected slugcats.
> **More clarification:**
> `ALL` will never hide any rooms.
> `ONLY` will *hide all rooms* if no slugcat is selected.
> `EXCEPT` will only hide conditionals set to `ONLY`.

### Creating a room
- Hover an empty area
- Press `R`
- Select room size
- Enter room name
- `Create`
- (See Droplet)
