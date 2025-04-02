# Falling Notes

A simple interactive music application where clicking or dragging creates falling dots. These dots play musical notes when they hit the bottom of the screen, with the scale determined by the vertical click position and the pitch by the horizontal position.

## How to Use

1.  **Open `index.html`:** Open the `index.html` file in a web browser.
2.  **Select a Scale:** Use the dropdown menu at the top left to choose a musical scale.
3.  **Create Notes:** Click anywhere on the main area of the screen (below the scale selector, outside the loop controls). A dot will appear and fall downwards.
4.  **Sound:** When a dot reaches the bottom, it will play a note corresponding to its horizontal position within the selected scale.
5.  **Looping:**
    *   **Enable:** Click the "Enable Loop Mode" button on the right panel.
    *   **Add Layer:** Click "Add Loop Layer" to create a new loop track (e.g., Loop 1).
    *   **Select:** Click the "Select" button on the desired loop layer to make it active for recording.
    *   **Record:** Click the "Record" button on the *selected* loop layer to start recording. Click again ("Stop Rec") to finish recording for that layer.
    *   **Play All:** Click "Play All" to start playback of all unmuted loops. The button will change to "Stop All". Click again to stop playback.
    *   **Mute/Unmute:** Click the "Mute" button on a loop layer to toggle its playback. Muted loops won't sound during "Play All".
    *   **Clear:** Click the "Clear" button on a loop layer to delete only its recorded notes.
    *   **Clear All Loops:** Click this button to delete *all* recorded notes from *all* layers.
    *   **Disable:** Click "Hide Loop Controls" to hide the panel and disable all looping functions.

## Features

*   **Interactive Music Creation:** Click on the screen to create falling notes.
*   **Musical Scales:** Choose between different musical scales (Major, Minor, Pentatonic, Blues, etc.) using the dropdown menu.
*   **Color-Coded Notes:** Notes are colored based on the selected scale, providing visual feedback.
*   **Multi-Layer Looping:**
    *   Record multiple independent loops of notes.
    *   Select specific loops to record into.
    *   Mute/unmute individual loops during playback.
    *   Clear individual loops or all loops at once.
    *   Play all active (unmuted) loops simultaneously.
*   Click and drag interaction.
*   Multiple musical scales selectable by vertical zones (Major, Major Pentatonic, Blues, Natural Minor, Harmonic Minor, Chromatic).
*   Horizontal position controls pitch within the selected scale (2-octave range).
*   Dot color correlates with scale (hue) and pitch (lightness).
*   Uses the Web Audio API for sound generation (sine waves).
*   Responsive zone layout (adjusts on window resize).
