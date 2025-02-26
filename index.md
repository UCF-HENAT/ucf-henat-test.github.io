---
layout: default
title: "HENAT Lab"
---

# HENAT Lab

<!-- Tab Navigation -->
<div class="tab">
  <button class="tablinks active" onclick="openTab(event, 'Research')">Research</button>
  <button class="tablinks" onclick="openTab(event, 'Publications')">Publications</button>
  <button class="tablinks" onclick="openTab(event, 'Teaching')">Teaching</button>
  <button class="tablinks" onclick="openTab(event, 'ProspectiveStudents')">Prospective Students</button>
  <button class="tablinks" onclick="openTab(event, 'Contact')">Contact</button>
</div>

<!-- Tab Content Sections -->
<div id="Research" class="tabcontent" style="display:block;">
  <h2>Research</h2>
  <p>Describe your research interests, projects, and innovations.</p>
</div>

<div id="Publications" class="tabcontent">
  <h2>Publications</h2>
  <p>List your key publications with links to full papers.</p>
</div>

<div id="Teaching" class="tabcontent">
  <h2>Teaching</h2>
  <p>Details about courses you teach and materials you provide.</p>
</div>

<div id="ProspectiveStudents" class="tabcontent">
  <h2>Prospective Students</h2>
  <p>Information for students interested in joining the HENAT Lab.</p>
</div>

<div id="Contact" class="tabcontent">
  <h2>Contact</h2>
  <p>Email: your-email@domain.com</p>
  <p>LinkedIn: <a href="https://linkedin.com/in/yourprofile">Your Profile</a></p>
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

<!-- CSS for Styling -->
<style>
  .tab {
    overflow: hidden;
    border-bottom: 2px solid #ddd;
    background-color: #f1f1f1;
    display: flex;
    justify-content: center;
  }
  .tab button {
    background-color: inherit;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 10px 20px;
    transition: 0.3s;
    font-size: 16px;
  }
  .tab button:hover {
    background-color: #ddd;
  }
  .tab button.active {
    background-color: #ccc;
    font-weight: bold;
  }
  .tabcontent {
    display: none;
    padding: 20px;
    border-top: none;
  }
</style>
