## Guidelines for a consistent DINA user interface

SUGGESTION 8/2017, NOT OFFICIAL

Major differences compared to previous Style guidelines at http://blog.dina-web.net/guidelines/style.html
- Simpler, less restrictive
- Discussion removed
- Expanded to include UI elements

--------------------------------

The goal of these guidelines is to help to create a visually and uniform set of DINA modules with consistently working user interfaces, so that users are not surprised or confused when transitioning between modules.

Guidelines can be used in various settings, such as:

*   web applications on both desktop and mobile devices
*   console applications
*   printed publications (part on visual style)
*   documentation

## Accessibility

Visual style should support good accessibility, and therefore particulary web content should conform as much as reasonable with the [W3C guidelines for web content accessibility](http://www.w3.org/TR/WCAG20/).

## Fonts

Requirements fo the fonts used in DINA applications:

*   Support for wide variety of languages and characters.
*   A serif, a sans serif and a fixed width “console font” should be part of the style. Those three types of fonts should harmonize.
*   Web fonts and TTF versions should exist (or be possible to create) for use on Windows, Linux, Mac providing same appearance regardless of OS used
*   Open license is required

**TODO**: Select the font(s).

Possible fonts:

*   **[Source Sans Pro](http://www.google.com/fonts/specimen/Source+Sans+Pro) / [Source Serif Pro](http://www.google.com/fonts/specimen/Source+Serif+Pro) / [Source Code Pro](http://www.google.com/fonts/specimen/Source+Code+Pro)**
*   **Google Noto** (with great support across cultures/languages)
*   **Lato** (currently used in user management module)


## Logo

![Logo](https://github.com/DINA-Web/dina_logo/blob/master/Dina%20final%20logo%20horizontal.png?raw=true)

Logo assets are available at [https://github.com/DINA-Web/dina_logo](https://github.com/DINA-Web/dina_logo).

Colors matching the logo:

**Dark green**

* RGB 19, 86, 51
* HEX #135633

**Medium green**

* RGB 30, 140, 67
* HEX #1e8c43

**Light green**

* RGB 116, 195, 116
* HEX #74c374

## Colors

For general visual design use white background, black text and dark green (see "Logo" above) as accent color.

For user actions and UI elements, use default Bootstrap 3 or equivalent colors. See for example https://getbootstrap.com/docs/4.0/components/buttons/

* Background: white and/or light grey
* Text: black
* Links: TBD (?)
* Actions
  * Primary/Save/Edit: bright blue
  * Warning/Cancel: yellow
  * Danger/Delete: red
  * Edit: greyish blue
* Messages
  * Success: green
  * Warning: yellow
  * Error: red
  * Information: greyish blue

## Customized colors

It is very easy to get colors wrong. It is perhaps more important to avoid the worst pitfalls than aiming at acheiving perfection.

Very good guidance when choosing colors that can be perceived clearly is provided by tools like [ColorBrewer 2](http://colorbrewer2.org).

*   For colors used, a harmonized and clearly perceivable selection of colors is required
*   No more than 7 steps and never more than 2 hues (if multihued) may be used, if users should be able to distinquish different colors
*   Aim for colorblind safe choices

With these requirements, the colors used in the DINA style will be guaranteed to be clearly perceived by most audiences across most media.

An example of a color profile that meets the above criteria is the following:

<font color="#ffffcc">█</font> <font color="#d9f0a3">█</font> <font color="#addd8e">█</font> <font color="#78c679">█</font> <font color="#41ab5d">█</font> <font color="#238443">█</font> <font color="#005a32">█</font>

Source: [http://colorbrewer2.org/](http://colorbrewer2.org/) (colorscheme with 7 steps, 2-color multihued yellow-green scale, colorblind safe)

A simple way to check that colors used make sense and can be distinguished is to convert to gray scale and check if different colors still can be discerned. A quick such test can ensure that you are in compliance with this guideline from W3C: [http://www.w3.org/TR/WCAG20/#visual-audio-contrast-without-color](http://www.w3.org/TR/WCAG20/#visual-audio-contrast-without-color)

For a more detailed check, tools like [Vischeck](http://www.vischeck.com/vischeck/) can be used to simulate how various kinds of color-blindness would affect perceptions of colors used in an image.

## UI elements

For buttons, use Windows-style order: Save on left, Cancel on right.

## CLI tools

CLI tools should display this message on startup:

<pre>DINA {tool name} - dina-project.net</pre>

**TODO**: Review the real message, or remove this part completely.
