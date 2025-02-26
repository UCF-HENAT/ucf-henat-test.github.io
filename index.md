---
layout: default
title: "HENAT Lab"
---

<!-- Tab Navigation (No Background) -->
<div class="tab">
  <button class="tablinks active" onclick="openTab(event, 'MengjieLi')">Mengjie Li</button>
  <button class="tablinks" onclick="openTab(event, 'Research')">Research</button>
  <button class="tablinks" onclick="openTab(event, 'Publication')">Publication</button>
  <button class="tablinks" onclick="openTab(event, 'Teaching')">Teaching</button>
  <button class="tablinks" onclick="openTab(event, 'ProspectiveStudents')">Prospective Students</button>
  <button class="tablinks" onclick="openTab(event, 'HENATLab')">HENAT Lab</button>
</div>

<!-- Tab Content Sections -->
<div id="MengjieLi" class="tabcontent" style="display:block;">
  <h2>Mengjie Li</h2>
  <p>Brief introduction about Mengjie Li, academic background, and research interests.</p>
</div>

<div id="Research" class="tabcontent">
  <h2>Research</h2>
  <p>Describe your research interests, projects, and innovations.</p>
</div>

<div id="Publication" class="tabcontent">
  <h2>Publication</h2>
  <p>List of key publications with links to full papers.</p>
</div>

<div id="Teaching" class="tabcontent">
  <h2>Teaching</h2>
  <p>Details about the courses you teach and educational contributions.</p>
</div>

<div id="ProspectiveStudents" class="tabcontent">
  <h2>Prospective Students</h2>
  <p>Information for students interested in joining HENAT Lab.</p>
</div>

<div id="HENATLab" class="tabcontent">
  <h2>HENAT Lab</h2>
  <p>Introduction to the HENAT Lab, its mission, members, and ongoing projects.</p>
</div>

<!-- JavaScript for Tab Switching -->
<script>
  function openTab(evt, tabName) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
      tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablinks");
    for (i = 0; i < tablinks.length; i++) {
      tablinks[i].className = tablinks[i].className.replace(" active", "");
    }
    document.getElementById(tabName).style.display = "block";
    evt.currentTarget.className += " active";
  }
</script>

<!-- CSS for Styling (No Background, Centered Tabs) -->
<style>
  .tab {
    overflow: hidden;
    display: flex;
    justify-content: center;
    border-bottom: 2px solid #ddd;
    padding: 10px 0;
  }
  .tab button {
    background-color: transparent;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 10px 20px;
    font-size: 18px;
    font-weight: bold;
    color: #000;
    transition: 0.3s;
  }
  .tab button:hover {
    text-decoration: underline;
  }
  .tab button.active {
    border-bottom: 3px solid #000;
  }
  .tabcontent {
    display: none;
    padding: 20px;
    text-align: left;
  }
</style>
