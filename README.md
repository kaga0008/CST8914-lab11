# CST8914 Lab 11: Accessible Custom Components & widgets
## Elizabeth Kaganovsky (040956095)

### 1. What is the keyboard interaction missing?
According to the ARIA authoring practices guide, all necessary functionality is present (enter/space to open a panel when the associated header has focus, tab/shift + tab to move back and forth between headers). However, some optional controls are unavailable:

- Up/down arrow: Synonymous with the functionality of tab/shift + tab, moves focus up and down respectively from one header in the accordion to the next.
- Home/end: Moves focus to the frist/last accordion header respectively.

Despite missing these, the necessary features are still including, making the accordion accesible by W3C standards.

### 2. What is the ARIA missing?
- aria-expanded="true" : Set to true/false to indicate if a panel is expanded or not.
- aria-controls="ID" : The ID of the panel controlled by the header.
- role="region" : Creates a landmark region that contains the expanded accordion panel to allow for ease of navigation with a screen reader.
- aria-labelledby="IDREF" : The ID of the header that controls the panel.