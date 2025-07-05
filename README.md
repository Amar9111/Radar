# Radar
Radar can use by mic
<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width,

initial-scale=1.0">

<title>Enhanced Radar Simulation</title>

<!-- Tailwind CSS CDN for easy styling -->

<script src="https://cdn.tailwindcss.com"></script>

<style>

/* Custom styles for the canvas and overall layout */

body {

font-family: 'Inter', sans-serif; /* Using Inter font as

per instructions */

overflow: hidden; /* Prevent scrollbars */

background-color: #0d0d0d; /* Dark background */

}

canvas {

display: block;

background-color: #000; /* Black background for radar */

border-radius: 1rem; /* Rounded corners for the canvas */

box-shadow: 0 0 20px rgba(0, 255, 0, 0.5); /* Green glow

effect */

touch-action: none; /* Disable default touch actions like

scrolling/zooming */

}

/* Styling for the info boxes */

.info-box {

background-color: rgba(0, 0, 0, 0.7);

border: 1px solid rgba(0, 255, 0, 0.5);

border-radius: 0.5rem;

padding: 0.75rem 1rem;

color: #00ff00;

font-family: 'monospace', sans-serif;

font-size: 0.9rem;

box-shadow: 0 0 10px rgba(0, 255, 0, 0.3);

}

/* Keyframe animation for pulse effect */

@keyframes pulse {

0% { transform: scale(1); opacity: 1; }

50% { transform: scale(1.05); opacity: 0.8; }

100% { transform: scale(1); opacity: 1; }

}

.pulse-animation {

animation: pulse 2s infinite ease-in-out;

}

/* Style for the audio meter */

#audio-meter-bar {
