<div id="top"></div>

[![GitHub all releases][release-shield]][release-url]
[![Wiki][wiki-shield]][wiki-url]
[![Issues][issues-shield]][issues-url]
[![Zero-Clause BSD][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

This code has been moved to: https://github.com/NeosoftTechnologiesInc/Open-DQMH-Request-Message-Diagram

# Open DQMH Request Message Diagram

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#Open DQMH Request Message Diagram">Open DQMH Request Message Diagram</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#how-to-use-it">How to use it?</a></li>
        <li><a href="#labview-shortcut-menu-plug-ins">LabVIEW Shortcut Menu Plug-ins</a></li>
      </ul>
    </li>
  </ol>
</details>

Adds a *Right-Click Shortcut* and a *Quick Drop Ctrl-Key Shortcut* (CTRL-K by default) to DQMH Module **Request** or **Request and Wait for Reply** or **Round Trip Broadcast** methods on the block diagram allowing the developer to quickly open the Message Diagram of the Message Handling Loop within the DQMH Module Main VI.

When writing code using **DQMH Framework**, you communicate with actors (DQMH Modules) by sending asynchronous or synchronous messages. Each DQMH Module has a set of methods, Public API VIs which are what you see on the block diagram, which collect the inputs for the message and transport it using LabVIEW user events. The actual logic that executes when the message is received resides in a Message Handling Loop (MHL) of the DQMH Module Main VI, which reads the message causes the corresponding subdiagram of the Case structure to execute. This subdiagram is called a "message diagram" because it corresponds to a message. 

During the development process it can be convinient for developpers to quickly access to the "message diagram" from the public method they use somewhere else. This LabVIEW IDE plugin retrievs selected subVIs on a diagram and if they are a part a the Public API VI of a DQMH opens the Main VI block diagram with the "message diagram" handling the message visible. Developpers have direct access to the business logic of the Request.

## Installation
- Download the Open DQMH Request Message Diagram.vip.
- Use VIPM to install it on your LabVIEW version (2020+).

## How to use it? 
- From a VI Block Diagram
- Right-click on a user DQMH Request and select
  - Open DQMH Request Message Diagram: this will open the Message Diagram of the Message Handling Loop within the DQMH Module Main VI
  <p align="center">
  <img src="https://github.com/Benji667/Open-DQMH-Request-Message-Diagram/blob/d530656174cae1ee0742d89b43d069c5dbbbbea2/img/OpenDQMHRequestMessageDiagram_ShortcutMenu.gif?raw=true" alt="Insert LVClass Property Node" width="50%" height="50%" pointer-events="none"/>
  </p>
- Launch the QuickDrop (Ctl+Space) and press
  - Ctl+k: this will open the Message Diagram of the Message Handling Loop within the DQMH Module Main VI
  <p align="center">
  <img src="https://github.com/Benji667/Open-DQMH-Request-Message-Diagram/blob/d530656174cae1ee0742d89b43d069c5dbbbbea2/img/OpenDQMHRequestMessageDiagram_QuickDrop.gif?raw=true" alt="Insert LVClass Property Node" width="50%" height="50%" pointer-events="none"/>
  </p>

## LabVIEW Shortcut Menu Plug-ins

To know more about LabVIEW Shortcut Menu Plug-ins: 
<a href="https://benjaminrlabviewextensions.github.io/LVMenu_Demo/" target="_blank">
  <img src="https://github.com/BenjaminRLabVIEWExtensions/Insert-LVClass-Property-Node/blob/54e9a5a032d7d5d79f9e4c9b9676f41238d953a7/img/hand-pointer-regular.svg?raw=true" width="14" height="14"/> Click here
</a>

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[release-shield]: https://img.shields.io/github/v/release/Benji667/Open-DQMH-Request-Message-Diagram?color=orange&logo=labview&style=for-the-badge
[release-url]: https://github.com/Benji667/Open-DQMH-Request-Message-Diagram/releases/tag/1.0.0
[wiki-shield]: https://img.shields.io/github/discussions/Benji667/Open-DQMH-Request-Message-Diagram?style=for-the-badge
[wiki-url]: https://github.com/Benji667/Open-DQMH-Request-Message-Diagram/wiki
[issues-shield]: https://img.shields.io/github/issues/Benji667/Open-DQMH-Request-Message-Diagram?style=for-the-badge
[issues-url]: https://github.com/Benji667/Open-DQMH-Request-Message-Diagram/issues
[license-shield]: https://img.shields.io/badge/LICENSE-Zero--Clause%20BSD-green?style=for-the-badge
[license-url]: https://github.com/Benji667/Open-DQMH-Request-Message-Diagram/blob/d530656174cae1ee0742d89b43d069c5dbbbbea2/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/benjaminrouffet/
