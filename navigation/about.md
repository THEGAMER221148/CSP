---
layout: post
title: About
permalink: /about/
comments: true
---

## As a conversation Starter

Here are some places I have lived.

<comment>
Flags are made using Wikipedia images
</comment>

<style>
    /* Style looks pretty compact, 
       - grid-container and grid-item are referenced the code 
    */
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
        gap: 10px;
    }
    .grid-item {
        text-align: center;
    }
    .grid-item img {
        width: 100%;
        height: 100px; /* Fixed height for uniformity */
        object-fit: contain; /* Ensure the image fits within the fixed height */
    }
    .grid-item p {
        margin: 5px 0; /* Add some margin for spacing */
    }

    .image-gallery {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 10px;
        }

    .image-gallery img {
        max-height: 150px;
        object-fit: cover;
        border-radius: 5px;
    }

    th {
        font-family: monospace
    }

    a {
      border-width: 5px;
      border-style: solid;
      border-radius: 5px;
      background-color: rgb(0, 128, 255);
      color: rgb(0, 64, 128);
      margin-top: 5px;
    }
</style>

<!-- This grid_container class is used by CSS styling and the id is used by JavaScript connection -->
<div class="grid-container" id="grid_container">
    <!-- content will be added here by JavaScript -->
</div>

<script>
    // 1. Make a connection to the HTML container defined in the HTML div
    var container = document.getElementById("grid_container"); // This container connects to the HTML div

    // 2. Define a JavaScript object for our http source and our data rows for the Living in the World grid
    var http_source = "https://upload.wikimedia.org/wikipedia/commons/";
    var living_in_the_world = [
        {"flag": "0/01/Flag_of_California.svg", "greeting": "Hey", "description": "California - forever (yeah this is the only place I've lived)"},
    ];

    // 3a. Consider how to update style count for size of container
    // The grid-template-columns has been defined as dynamic with auto-fill and minmax

    // 3b. Build grid items inside of our container for each row of data
    for (const location of living_in_the_world) {
        // Create a "div" with "class grid-item" for each row
        var gridItem = document.createElement("div");
        gridItem.className = "grid-item";  // This class name connects the gridItem to the CSS style elements
        // Add "img" HTML tag for the flag
        var img = document.createElement("img");
        img.src = http_source + location.flag; // concatenate the source and flag
        img.alt = location.flag + " Flag"; // add alt text for accessibility

        // Add "p" HTML tag for the description
        var description = document.createElement("p");
        description.textContent = location.description; // extract the description

        // Add "p" HTML tag for the greeting
        var greeting = document.createElement("p");
        greeting.textContent = location.greeting;  // extract the greeting

        // Append img and p HTML tags to the grid item DIV
        gridItem.appendChild(img);
        gridItem.appendChild(description);
        gridItem.appendChild(greeting);

        // Append the grid item DIV to the container DIV
        container.appendChild(gridItem);
    }
</script>

### Journey through Life

I was born in Los Angeles but moved to San Diego with my mom and two brothers when I was <strong>4</strong>. I skipped 3rd grade when I was 8 and also gained a love for programming. I moved a few more times around the same area and now live here!

### Hobbies

I have a few hobbies:

 - talking to my friends
 - making digital music
 - playing my drums
 - coding
 - roller coasters

### My games

My passion for game development has led me to make games (I know, real shocker). Here are some links to games and platform accounts i have made:

 - <a href="https://scratch.mit.edu/users/weststefany/">My Scratch page</a>
 - <a href="https://west-coast-games.itch.io/">My Itch.io page</a>
 - <a href="https://westcoastgames.net/">My website</a>
 - <a href="https://github.com/THEGAMER221148">My GitHub page</a>
 - <a href="https://rcbonline.net/">Roller Coaster Builder 2</a>


<!-- <comment>
Gallery of Pics, scroll to the right for more ...
</comment>
<div class="image-gallery">
  <img src="{{site.baseurl}}/images/about/missionary.jpg" alt="Image 1">
  <img src="{{site.baseurl}}/images/about/john_tamara.jpg" alt="Image 2">
  <img src="{{site.baseurl}}/images/about/tamara_fam.jpg" alt="Image 3">
  <img src="{{site.baseurl}}/images/about/surf.jpg" alt="Image 4">
  <img src="{{site.baseurl}}/images/about/john_lora.jpg" alt="Image 5">
  <img src="{{site.baseurl}}/images/about/lora_fam.jpg" alt="Image 6">
  <img src="{{site.baseurl}}/images/about/lora_fam2.jpg" alt="Image 7">
  <img src="{{site.baseurl}}/images/about/pj_party.jpg" alt="Image 8">
  <img src="{{site.baseurl}}/images/about/trent_family.png" alt="Image 9">
  <img src="{{site.baseurl}}/images/about/claire.jpg" alt="Image 10">
  <img src="{{site.baseurl}}/images/about/grandkids.jpg" alt="Image 11">
  <img src="{{site.baseurl}}/images/about/farm.jpg" alt="Image 12">
</div> -->

<html lang="en">
    <p>📊 Scoring Guide:</p>
<ul>
  <li>1 = .55 - Self-management (Taking ownership)</li>
  <li>2 = .75 - Incremental progression (Step-by-step growth)</li>
  <li>3 = .85 - Self-organization (Time &amp; priority management)</li>
  <li>4 = .90 - Iterative techniques (Continuous refinement)</li>
  <li>5 = +.01 per quality delivery - Continuous delivery (Consistent contribution)</li>
  <li>Mastered-Y = .93 - Excellence in all areas</li>
</ul>

<hr />

<h4 id="-evaluation-matrix">📊 Evaluation Matrix</h4>

<table>
  <thead>
    <tr>
      <th>Skill</th>
      <th>Mastered (Y/N)</th>
      <th>Self Rank (1-5)</th>
      <th>Peer Rank (1-5)</th>
      <th>Teacher Rank (1-5)</th>
      <th>Average</th>
      <th>Notes/Evidence</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>🎯 Core Behaviors</strong></td>
      <td>Y</td>
      <td>5</td>
      <td>5</td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Attendance</td>
      <td>[]</td>
      <td>5</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Work Habits</td>
      <td>[ ]</td>
      <td>4.5</td>
      <td>0</td>
      <td>0</td>
      <td>0.0</td>
      <td> </td>
    </tr>
    <tr>
      <td>Behavior</td>
      <td>[]</td>
      <td>5</td>
      <td>4.5</td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Timeliness</td>
      <td>[]</td>
      <td>5</td>
      <td> </td>
      <td>0</td>
      <td>0.0</td>
      <td> </td>
    </tr>
    <tr>
      <td><strong>💻 Technical Skills</strong></td>
      <td>[]</td>
      <td>5</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Tech/Cyber Sense</td>
      <td>[]</td>
      <td>5</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Tech/Cyber Talk</td>
      <td>[]</td>
      <td>4.5</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>I've still got some terminology to learn</td>
    </tr>
    <tr>
      <td>Tech Growth</td>
      <td>[]</td>
      <td>5</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td><strong>🤝 Collaboration</strong></td>
      <td>[]</td>
      <td>4.5</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>I'm very used to idependent work, so I have to practice collaboration skills a little more</td>
    </tr>
    <tr>
      <td>Advocacy</td>
      <td>[]</td>
      <td>5</td>
      <td>0</td>
      <td>0</td>
      <td>0.0</td>
      <td> </td>
    </tr>
    <tr>
      <td>Communication &amp; Collab</td>
      <td>[]</td>
      <td>5</td>
      <td>0</td>
      <td>0</td>
      <td>0.0</td>
      <td> </td>
    </tr>
    <tr>
      <td><strong>🎨 Professional Skills</strong></td>
      <td>[]</td>
      <td>4.5</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Integrity</td>
      <td>[]</td>
      <td>5</td>
      <td>0</td>
      <td>0</td>
      <td>0.0</td>
      <td> </td>
    </tr>
    <tr>
      <td>Organization</td>
      <td>[]</td>
      <td>4.5</td>
      <td>0</td>
      <td>0</td>
      <td>0.0</td>
      <td> </td>
    </tr>
    <tr>
      <td><strong>📈 TOTALS</strong></td>
      <td> </td>
      <td><strong>72.5</strong></td>
      <td><strong>0</strong></td>
      <td><strong>0</strong></td>
      <td><strong>0.0</strong></td>
      <td> </td>
    </tr>
    <tr>
      <td><strong>🎯 AVERAGE SCORE</strong></td>
      <td> </td>
      <td><strong>0.0</strong></td>
      <td><strong>0.0</strong></td>
      <td><strong>0.0</strong></td>
      <td><strong>0.0</strong></td>
      <td> </td>
    </tr>
  </tbody>
</table>

</html>