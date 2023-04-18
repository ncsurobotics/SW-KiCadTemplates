# SW-KiCad-Templates

Template board files for various stackups. Can be imported for other boards.



## Using Templates

- Open your PCB
- Open Board Settings
- Choose Import Settings from Another Board
- Choose one of the template boards


## Creating a Template

- Find the capabilities and stackup info from your PCB manufacturer
- Create a new kicad project. Delete the schematic. Keep the pcb file.
- Add the kicad gitignore to the folder of your new template
- Edit the pcb file. Open board settings.
- Board Stackup
    - Generally, do not edit board layers in the "Board Layers Editor"
    - Physical Stackup
        - Choose number of copper layers
        - Check impedance controlled if applicable
        - Edit dielectric constants (epsilon R)
        - Choose board thickness
        - Generally, leave colors unspecified
        - Click "Adjust Dielectrick Thickness" button
    - Generally, don't edit Board Finish settings (for templates). These may be changed per board sometimes.
    - Solder Mask / Paste
        - Edit all values to match manufacturer capabilities
        - If not specified by manufacturer, leave defaults
- Text and Graphics
    - No changes need to be made. Defaults are fine.
    - Changes made here should be per-board not template.
- Design Rules
    - Constraints
        - Fill in everything your manufactuerer specifies
    - Make no changes in other sections (that should be per-board not template)
