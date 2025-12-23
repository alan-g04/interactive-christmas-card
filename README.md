# Snoopy’s Festive Pixel Decorator

An interactive, browser-based Christmas experience featuring Peanuts-inspired pixel art. This project demonstrates efficient canvas rendering, state-driven UI, and procedural asset generation within a single HTML file.

## Features

  Procedural Generation: The Christmas tree is generated programmatically using a "jagged triangle" algorithm to create a unique, pixelated texture every time the script runs.

  Interactive Decorating: A custom-built coordinate mapping system (`SLOT_COORDS`) allows users to place and remove ornaments on specific branches.

  Animation: Frame-based animations for Snoopy and Woodstock, including binary state changes upon completion.

  Web Audio API: Synthesised sound effects (sine and triangle waves) for interactions, avoiding the need for external MP3/WAV files.

  Snapshot Capability: Utilises `canvas.toDataURL()` to allow users to save their decorated tree as a `.png` file.

## Technical Overview

  Rendering: Uses a 320x400 canvas with `image-rendering`: pixelated to maintain crisp edges regardless of display scaling.

  State Management: A central state object tracks the application's progress, including decoration indices and the "won" boolean.

  Maths Integration: Confetti and snow particles use basic physics (velocity and gravity vectors) to simulate movement.

## Customisation

To personalise the card, locate the `YOUR_MESSAGE` constant at the beginning of the `<script>` block:

    const YOUR_MESSAGE = 'Happy Christmas, [Name]!';

You can also adjust the `WIN_THRESHOLD` if you wish to change how many decorations are required to reveal the final message.

## Installation & Usage

1. Save the code as `index.html`.

2. Open the file in any modern web browser.

3. No dependencies or local servers are required — the entire application is self-contained. Merry Christmas!!
