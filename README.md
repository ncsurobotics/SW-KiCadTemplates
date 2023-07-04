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
- Create a readme in the folder with a more detailed explanation of the template's configuration

<hr />

- Edit the pcb file. Open board settings.
- NOTE: You can import settings from another template as a starting point if you want
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
    - Defaults
        - Change all default sizes based on what makes sense for the board's manufacturing process
        - If in doubt, use values from the JLCPCB 2 layer 1.6mm board template
        - Make sure default unit of mils is used
    - Formatting: No changes
    - Text Variables: No changes
- Design Rules
    - Constraints
        - Fill in everything your manufactuerer specifies
    - Make appropriate chances in the default netclass section
    - Make no changes in other sections (that should be per-board not template)
