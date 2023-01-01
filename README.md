# Welcome to Ebullientworks Obsidian Theme 👋 [![GitHub tag (Latest by date)](https://img.shields.io/github/v/tag/ebullient/obsidian-theme-ebullientworks)](https://github.com/ebullient/obsidian-theme-ebullientworks/releases) ![GitHub all releases](https://img.shields.io/github/downloads/ebullient/obsidian-theme-ebullientworks/total?color=success)

<table><tr><td>Jump: </td>
<td><a href="#style-settings">Settings</a></td>
<td><a href="#admonitions-and-callouts">Admonitions</a></td>
<td><a href="#tables">Tables</a></td>
<td><a href="#embeds">Embeds</a></td>
<td><a href="#colors">Colors</a></td>
<td><a href="#creating-your-own-accent-colors">Custom accents</a></td></tr></table>

![](https://raw.githubusercontent.com/ebullient/obsidian-theme-ebullientworks/main/images/ebullientworks-theme.jpg)

This is a dark and light theme for [Obsidian.md](https://obsidian.md), a note taking app. 

Headers are styled and sized (for mobile and not) with and without stacked tabs. Modals, tables, and other panels are also styled. 

Some light styling has also been applied for the following community plugins: 

- admonition
- calendar
- day planner
- sliding panes
- timelines
- tracker

This theme is compatible with custom task snippets from the [Snippitor](https://github.com/ebullient/obsidian-snippetor).

## Style Settings

This theme does support style settings. Settable attributes: 

- (0.3.25) "Suppress/remove this theme's checkbox styles"
    Set this to true if you are going to use your own task snippet (💡 Check out [Snippetor](https://github.com/ebullient/obsidian-snippetor)!)

- (0.5.x) "View header actions to the left"
    Set this to true if the view header is visible, and you want the controls on the left side of the tab contents, rather than the right.

- "Show external links in edit mode"
    If true, external links (or the content of markdown links) will be shown in edit mode. External links are hidden by default.

- (0.1.8) "Float front-matter in a box to the right"
    If true, front-matter in preview mode will be collapsed in a top-right container.

- (0.5.x) "Hide the heading used to embed a document"
    If true, the heading used to embed a document will be hidden.

- Custom Fonts

    - "Headings"
        Font variant for text headings (h1 to h6)

    - (0.3.24) "Heading Font Caps Variant"
        Capitalization variant for text headings (h1 to h6)

    - "Tags"
        Font for displaying inline tags; empty will use default text font

- Colors
    This allows you to select the primary or secondary color from the colors in the palette (purple, pink, green, teal, or blue). You can also select a "custom" accent color, in which case, you should define and enable your own snippet as described below.

    - "Primary accent color" 
        Choose the primary accent color. You should define a snippet if you select primary-accent-custom. See the Theme's README.

    - "Secondary accent color"
        Choose the secondary accent color. You should define a snippet if you select secondary-accent-custom. See the Theme's README.

## Removed

- (added in 0.3.4, removed in 0.5.*) Use default theme list indent
    This theme condenses whitespace padding in ordered and unordered lists. This toggle allows you to use list spacing from the default theme.

- (removed in 0.5.x) Show / Hide, the section was removed (remaining contents flattened with the first section)

- (added in 0.2.8, removed in 0.5.x) "Hide collapse indicators unless hovered or active"
    If true, hide collapse indicators in all three modes unless they are hovered over or the line is active.

- (added in 0.3.13, removed in 0.5.x) Show collapsed sidebars on hover
    If true, when the left or right sidebar is in a collapsed state, you can temporarily display (and interact) with its content by hovering over the ribbon. 

- (0.3.26) Removed other font settings. 
    Use Obsidian Appearance to set text and monospace fonts.

- (added in 0.2.7, removed in 0.5.x) Tag brightness (dark/light mode)
    Select a brightness or contrast level for tags. In 0.5.x and above, the accent color from appearance settings is used as the tag color (reset the value to see the theme default).

## Admonitions and callouts

As of version 6.5.1, you can disable the color picker for admonitions (globally or per-admonition) to have colors picked up from CSS styles instead. All of the default admonitions, in addition to two additional custom types, have been styled.

Those two custom types are:

- `reference`  
    Styled for inline reference metadata. Compact, monospace font.  
    To use this style, create a `reference` admonition (I recommend you use the closed book icon, but take your pick).
    
- `toc`
    Styled to create a floating (hover:right) section for Table of Contents
    To use this style, create a `toc` admonition (I recommend you use the list icon, but take your pick).
    
Here is what they look like (Callouts and Admonitions): 

![](images/admonitions.png)

## Tables

![](images/table-styles.png)

To constrain table content to the width of the pane, use: 
```
---
cssclass: force-wrap
---
```

To prevent column headers from wrapping, use: 
```
---
cssclass: word-wrap
---
```

## Embeds

To make embedded content "invisible" (same background color as the including page and much less padding), use the `invisible-embed` css class:

```
---
cssclass: invisible-embed
---
```

## Colors

All colors are sourced from [this palette](https://accessiblepalette.com/?lightness=98.2,93.9,87.5,82.5,74.8,66,48.4,30.6,19.4,10&C76E85=0,0&DD5755=0,0&d78e6e=0,-8&E1BA60=0,-10&5c7a62=0,0&3376AD=0,10&8E6787=0,0&808080=0,0&009698=0,-3)

<table>
<tr><td>
<img width="349" alt="image" src="https://user-images.githubusercontent.com/808713/210182009-f41561f6-62b1-47df-b6bb-8d5c4531d934.png">
</td><td>
<img width="340" alt="image" src="https://user-images.githubusercontent.com/808713/210182020-3cbbda60-06ff-42db-b589-810a8f7d084d.png">
</td></tr>
</table>

### Creating your own accent colors

A simple way to select colors that will work with this palette is by applying a grayscale filter to a selected hue. 

1. Use the following URL to apply the grayscale filter to a color of your choice: 
https://grayscale.design/app?lums=71.05%2C60.94%2C48.16%2C35.39%2C17.24%2C6.39%2C2.80&palettes=%235c7a62%2C%238e6787&filters=0%7C0%2C0%7C0&names=green%2Cpurple&labels=%2C

2. Create a snippet that contains your customized colors. 

#### Example

For example, let's use a REALLY BOLD RED: `#ae2012`.

1. If we visit the link above, we can scroll down a bit until we see a button "Add a color", and we paste this value (including the `#` in that field). This will show us something like this:

![](images/create-a-custom-accent-color.png)

2. Scroll down until you see `Step 3`, which is the step you need to export your colors. You'll want to use the CSS variables.

    If we want to use this red as the primary color: 
    ```
    .primary-accent-custom {
        --primary-accent-0: rgb(250, 210, 206); /* red-100 */
        --primary-accent-1: rgb(248, 192, 187); /* red-200 */
        --primary-accent-1-rgb: 248, 192, 187;  /* Note removal of rgb() function */
        --primary-accent-2: rgb(245, 163, 156); /* red-300 */
        --primary-accent-3: rgb(241, 127, 117); /* red-400 */
        --primary-accent-4: rgb(222, 40, 23);   /* red-500 */
        --primary-accent-4-rgb: 222, 40, 23;    /* Note removal of rgb() function */
        --primary-accent-5: rgb(142, 25, 15);   /* red-600 */
        --primary-accent-6: rgb(95, 17, 10);    /* red-700 */
    }
    ```

    If we want to use this red as the secondary color:
    ```
    .secondary-accent-custom {
        --secondary-accent-0: rgb(250, 210, 206); /* red-100 */
        --secondary-accent-1: rgb(248, 192, 187); /* red-200 */
        --secondary-accent-1-rgb: 248, 192, 187;  /* Note removal of rgb() function */
        --secondary-accent-2: rgb(245, 163, 156); /* red-300 */
        --secondary-accent-3: rgb(241, 127, 117); /* red-400 */
        --secondary-accent-4: rgb(222, 40, 23);   /* red-500 */
        --secondary-accent-4-rgb: 222, 40, 23;    /* Note removal of rgb() function */
        --secondary-accent-5: rgb(142, 25, 15);   /* red-600 */
        --secondary-accent-6: rgb(95, 17, 10);    /* red-700 */
    }
    ```

3. Create a snippet (e.g. a file named`accent-colors.css`) containing this content in the `.obsidian/snippets` directory. Go to the Obsidian Appearance settings use the refresh button if necessary to find the snippet, and enable it. Provided you've selected the "custom" value in the primary/secondary style settings drop-down, you should be off to the races with this brilliant red.


### Changing tag colors

As of 0.5.3 (Obsidian 0.16+ / 1.x), use the "accent color" setting on the appearance pane to set your tag color. Resetting the value will use the theme default.

For 0.2.7 through 0.5.2, you can alter the color contrast (against the usual scale, 0-6) for tags in light or dark mode. 

## Credits

I've begged/borrowed/stolen CSS snippets from just about everywhere, but I started from vanilla and tried to be judicious about what to include to keep things lean. 

I frequently reference the following two themes, as they're often the quickest to consume a new CSS trick or snippet: 

- [Spectrum](https://github.com/Braweria/Spectrum)
- [ITS Theme](https://github.com/SlRvb/Obsidian--ITS-Theme)

If you have ideas or requests, please open an issue. ;)

<a href="https://www.buymeacoffee.com/ebullient" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
