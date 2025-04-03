# Falling Notes

A simple interactive music application where clicking or dragging creates falling dots. These dots play musical notes when they hit the bottom of the screen, with the scale determined by the vertical click position and the pitch by the horizontal position.

## How to Use

1.  **Open `index.html`:** Open the `index.html` file in a web browser.
2.  **Create Notes:** Click or drag anywhere on the main area of the screen. Dots will appear and fall downwards.
3.  **Sound:** When a dot reaches the bottom, it will play a note corresponding to its horizontal position within a scale determined by its vertical starting position.
4.  **Looping:**
    *   **Enable/Disable:** Click the "Enable Loop Mode" button on the right panel to show the controls. Click "Disable Loop Mode" to hide them.
    *   **Add Layer:** Click "Add Loop Layer" to create a new loop track.
    *   **Select:** Click the "Select" button on the desired loop layer to make it active for recording.
    *   **Record:** Click the "Record" button on the *selected* loop layer to start recording. Clicks or drags will add notes to this loop. Click "Stop Rec" to finish recording. *The loop's duration is determined by the time of the last note recorded.* 
    *   **Playback Mode (Sync/Async):** Use the toggle button ("Sync ON" / "Async ON") to switch between playback modes *before starting playback*:
        *   **Sync ON:** All active loops start together and restart based on the duration of the *longest* loop. Shorter loops will wait for the longest loop to finish before restarting.
        *   **Async ON:** Each active loop starts and restarts independently based on its *own* duration.
    *   **Play All / Stop:** Click "Play All" to start playback of all unmuted loops in the currently selected mode (Sync or Async). The button changes to "Stop". Click "Stop" to halt all playback.
    *   **Mute/Unmute:** Click the "Mute" button on a loop layer to toggle its playback.
    *   **Clear Layer:** Click the "Clear" button on a loop layer to delete only its recorded notes.
    *   **Clear All Loops:** Click this button to delete *all* recorded notes from *all* layers and add one new empty loop layer.

## Features

*   **Interactive Music Creation:** Click or drag on the screen to create falling notes.
*   **Vertical Zones for Scales:** The vertical starting position determines the musical scale (Major, Pentatonic, Blues, Minor, etc.).
*   **Horizontal Position for Pitch:** The horizontal starting position determines the pitch within the selected scale (3-octave range from C2 to C5).
*   **Color-Coded Notes:** Notes are colored based on the scale (hue) and pitch (lightness).
*   **Multi-Layer Looping:**
    *   Record multiple independent loops.
    *   Select specific loops for recording.
    *   Mute/unmute individual loops.
    *   Clear individual loops or all loops at once.
    *   **Synchronous & Asynchronous Playback:** Choose between Sync (all loops aligned) and Async (loops play independently) modes.
    *   Loop duration based on the last note played, eliminating trailing silence.
*   Uses the Web Audio API for sound generation (sine waves).
*   Click and drag interaction.
*   Multiple musical scales selectable by vertical zones (Major, Major Pentatonic, Blues, Natural Minor, Harmonic Minor, Chromatic).
*   Dot color correlates with scale (hue) and pitch (lightness).
*   Responsive zone layout (adjusts on window resize).
