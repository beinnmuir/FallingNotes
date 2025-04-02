# Falling Notes

A simple interactive music application where clicking or dragging creates falling dots. These dots play musical notes when they hit the bottom of the screen, with the scale determined by the vertical click position and the pitch by the horizontal position.

## How to Use

1.  Open `index.html` in your web browser.
2.  The screen is divided into horizontal zones, each labeled with a musical scale (e.g., Major, Blues, Minor).
3.  Click or click-and-drag anywhere on the screen:
    *   **Vertical Position (Zone):** Determines the musical scale of the note played.
    *   **Horizontal Position (Left-to-Right):** Determines the pitch of the note within the selected scale (lower notes on the left, higher notes on the right).
4.  Each falling dot has a color:
    *   **Hue (Base Color):** Indicates the musical scale zone.
    *   **Lightness:** Indicates the pitch (lighter on the left, darker on the right).
5.  Listen as the dots reach the bottom and create melodies!

## Features

*   Click and drag interaction.
*   Multiple musical scales selectable by vertical zones (Major, Major Pentatonic, Blues, Natural Minor, Harmonic Minor, Chromatic).
*   Horizontal position controls pitch within the selected scale (2-octave range).
*   Dot color correlates with scale (hue) and pitch (lightness).
*   Uses the Web Audio API for sound generation (sine waves).
*   Responsive zone layout (adjusts on window resize).
