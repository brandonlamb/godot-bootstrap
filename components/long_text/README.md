# GUI elements: `long_text`

Displays very long text in a pleasing way.  Replaces use of a `Label` for when
you need long descriptive text.  It separates paragraphs with either actual
new line characters, or the string "\n".  It currently does not support
BIDI text.

It uses the Label theme for display.

It expects to be embedded inside a ScrollContainer, but doesn't have to.

![example](long_text.png)

**Category**: `gui`


## Usage

Add a `Container` to where you want the text to be inserted, then select the
`long_text.gd` as the corresponding script object.

The following attributes can be set:

* **Indent Pixels** (`int::indent_pixels`) - how any pixels to use as the
  first line indention for each paragraph.
* **Paragraph Separation** (`float::paragraph_separation`) - font height
  multiplier for the separation between paragraphs. `1.0` means each paragraph
  is separated by a full text height, `0.5` means they are separated by half
  a text height.
* **Line Height** (`float::line_height`) - font height multiplier for
  each line of text's height.  `0.5` means that the lines overlap each other,
  `2.0` means double-spaced lines.
* **Color** (`Color::color`) - text color.  If not set, the theme color for the
  Label text will be used.
* **Font** (`Font::font`) - text font.  If not set, the theme font for the Label
  text will be used.
* **Text** (`String::text`) - text to display.


