An [nx-hbmenu](https://github.com/switchbrew/nx-hbmenu) redesign, aiming to continue the "ocean" trend of previous homebrew launchers while also incorporating the modern, minimalist feel of the Nintendo Switch system UI.

* [Themes](#themes)
* [Layout](#layout)
* [Text](#text)
* [Colors](#colors)
* [Assets](#assets)
* [Icons](#icons)
* [Wave Effect](#wave-effect)
* [Todo](#todo)

Note: The measurements and assets provided assume that the hbl menu will be rendered at 720p in both handheld and console mode.

### Themes

The intention was for hbl to match the user's current Switch theme, so two (somewhat) matching themes are provided:

**Dark Theme**

![dark theme](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/mockups/dark/inline.png)

**Light Theme**

![light theme](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/mockups/light/inline.png)

### Layout

UI elements are aligned to a 20x20 pixel grid (the red lines in the mockups below mark 8 grid spaces). The elements in each corner of the screen are given relatively generous margins to avoid [cropping / overscan issues](https://www.engadget.com/2010/05/27/hd-101-overscan-and-why-all-tvs-do-it/) when displayed on TV screens:

![grid layout](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/guides/grid.png)

### Text

Besides the "hbl" logo, all text use the open-source [Inter UI](https://github.com/rsms/inter) font family, in a total of 4 different size/weight combinations:

* **42px medium** - titles
* **28px medium** - clock, directory path, and action prompts
* **24px regular** - main text, used for the app description
* **20px regular** - secondary information, like the version string and app author / size

![text layout](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/guides/text.png)

The "hbl" logo text is custom and will be available in SVG format once it has been finalised :)

### Colors

| Dark Theme | Light Theme |
|:-|:-|
|![dark theme swatch](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/guides/swatches/dark.png)| ![light theme swatch](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/guides/swatches/light.png) |

As text for convinience:
 
**Dark Theme:** `#2D3742`, `#60CCCC`, `#429A9F`, `#6783C9`, `#516EAD`, `#2D98AF`, `#FFFFFF`, `#C0C0C3`

**Light Theme:** `#EBF0F6`, `#65D4FA`, `#6BB9FF`, `#97AEFF`, `#8088EA`, `#61B6EE`, `#222222`, `#888892`

### Assets

Image assets for the hbl logo and various UI elements like shadows, gradients, etc are provided in [`/assets`](https://github.com/jaames/switch-hbl-mockup/tree/master/assets), and are aligned as shown:

![slices](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/guides/slices.png)

### Icons

Homebrew app icons should be *at least* 220x220 px for the large "details" view, but ideally around 300x300 or more to allow for future layouts with larger icons.

List icons are 140x140 and the selected icon is scaled up to 160x160. 

### Wave Effect

The wave motion should be *extremely* subtle and calm, with maxiumum wave amplitude being no higher than ~8px or so. Otherwise it may be too distracting (and cause motion sickness :P).

In total there are 4 wave layers, with the order of `primary color`, `primary shadow color`, `secondary color` and `secondary shadow color` from front to back. Waves should not have transparency unless specified in the theme.

The lower 180px of the wave fades into a slighty deeper color (`wave gradient` in the color swatches). This is to both give the "water" a sense of depth and to ensure that the lower text is readable:

![wave](https://raw.githubusercontent.com/jaames/switch-hbl-mockup/master/guides/wave.png)

### Todo

* Alternate grid layout
* Full homebrew launcher logo
* Sample app icons that follow the same aesthetic?
* Website landing page redesign?
