Using the GUI:

After running the SISC algorithm (written in python) from Automanner, place the patterns in a created folder name Data with a desired name.

Dependency

- jquery
- papa parse
- amcharts
- bootstrap
- THREE.js
- OrbitalControls.js

Usage Instruction:

Use one of the following three combinations to display the UI in a PHP enabled webpage:

demo.php + demo.css + demo.js (for demo purposes, shows all the patterns with no embded survey)
gui.php + gui2.css + gui2.js (for running live studies, embeds a google survey, speeds up the video when playing normally, unlocks parts of the survey according to user interaction)
turkgui.php + gui.css + gui.js  (for running mechanical turk studies, generates a session key upon worker completion, encodes id into a base64 string, forces user to annotate each pattern and stores the results in a mysql database)

Access your pattern by (demo|gui|turkgui).php?id=(name of the pattern folder - encode it to a base64 string for turkgui.php)

Change the links in the php files(gui.php|turkguio.php) accordingly for collecting data with google form surveys.

Code Description: 

demo.php|gui.php|turkgui.php - uses amcharts to display timeline and pie graph, embeds custom google survey for collecting data, uses html5 video to display a webm/mp4 video 

gui.js|gui2.js - uses three.js to create and render a skeleton extracted from the data generated from the SISC algorithm, plots the patterns in a timeline from the given segments, traverse/replays the given segments based on user interaction (when a user clicks on the segment) 

demo.css|gui.css|gui2.css - styles the web pages accordingly
