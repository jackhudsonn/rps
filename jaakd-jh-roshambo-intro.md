---
layout: default
title: "Rock Paper Scissors: Expert Mode"
heading: "Rock Paper Roshambo in JavaScript"
subheading: "Game History"
description: "Roshambo on Expert Mode"
user-story: "As a player, I want to play Roshambo against the computer and view my game history so that I can see the results of my previous games."
---

<p>Which one will it be?</p>
<a href="#" onclick="playRoshambo('scissors')">scissors</a>
<a href="#" onclick="playRoshambo('rock')">rock</a>
<a href="#" onclick="playRoshambo('paper')">paper</a>

<br/>
<div id="results"></div>
<script>

playRoshambo = function(clientGesture){
    if (clientGesture=='scissors') {
        result = "lose";
    } // end if

    if (clientGesture=='paper') {
        result = "tie";
    } // end if

    if (clientGesture=='rock') {
        result = "win";
    } // end if

    document.getElementById('results').innerHTML = result;
} // end method

</script>
