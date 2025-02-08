# LayoutRadioGenerator
Creates a radio that let you switch through multiple template layouts.
You can rearange position, size and orientation of each control to create different layouts to select from.
The generator traverses the group hierachy, so you can also resize and reposition groups/pagers/grids and the controls within.

**Note that manipulation of the control tree cannot be tracked** 

In particular, it is not possible to apply following changes between layouts:
  - moving controls in and out of groups or pagers
  - create or delete controls
  - change the Front/Back position (aka *Arrangement*) of controls
## Usage
  1. add the Layouter group to your template.
  2. arrange the controls to a suitable layout. You can reposition controls and change their size and orientation. 
  3. run the template, press "Add". Stop the template and repeat Step 2.
  4. After adding all layouts, copy the "LayoutRadio" from the Layouter to your template and remove the Layouter.

## Functions
  - **Add**: Adds a layout to the LayoutRadio.
  - **Update**: Sets the templates layout at the radio's selected position.
  - **Remove**: Removes the layout at the radio's selected position.
  - **Clear**: Removes all layouts from the radio.
