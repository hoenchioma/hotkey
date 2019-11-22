# Hotkey
A cross platform solution for controlling your PC from a mobile device
(This is a university project for the course CSE-2216 (Application Development Lab) at University of Dhaka.)

This application is in essence an all in one solution to control your desktop computer from a mobile device. This app aims to be a simple, minimalistic and easy to use way to control your desktop when you are unable to physically do it yourself.
Not only does it provide the conventional mouse and keyboard support, it also provides easy interfaces for directly controlling presentation software, pdf readers, media players and much much more.

## Features

An exhaustive list of all currently available features and components in our application are as follows:
### Connection: 
There are 2 main modes of connecting the mobile and desktop (server) applications.
1. WiFi/LAN: If both devices are under the same Local Area Network (LAN) via WiFi or ethernet, this connection mode is available.
1. Bluetooth: If the mobile device as well as the desktop device supports bluetooth, this connection mode is available. Both methods use QR code for doing the authentication and handshake (so that the user does not have to manually enter any address).
### General Control:
1. Keyboard emulation: Emulate keyboard
2. Mouse/touchpad emulation: Emulated mouse via touchpad like interface
3. Live screen feed: See a live feed of the desktop screen while controlling. You can also interact (move and click the cursor) while using this mode.
### Special Control:
1. Presentation/Powerpoint assistant: This has facilities such as enter/exit slide show, goto next/previous slide, etc. It even has the feature of using a virtual laser pointer which can be moved by the app.
2. PDF reader: Next/previous page, fullscreen, layout fit width/height, goto page, etc.
3. Gamepad: Has a gamepad layout like layout with configurable buttons (mappable to keyboard keys).
4. Custom macros: One can save certain key combinations for faster use in certain situations.
5. Media keys: contains buttons for invoking the hardware buttons for play, pause, skip next, skip previous, volume up, volume down, etc.

## Members/Collaborators:
1. Raheeb Hassan (`Roll: AE-42`)&nbsp;&nbsp;&nbsp;<a href="https://github.com/hoenchioma"><img src="https://image.flaticon.com/icons/png/512/25/25231.png" width="20" height="20"/></a>&nbsp;&nbsp;&nbsp;<a href="mailto:raheeb@myself.com"><img src="http://www.clker.com/cliparts/5/S/U/Y/A/R/email-icon-th.png" alt='Email Icon clip art' width="20" height="20"/></a>
2. Farhan Kabir (`Roll: AE-12`)&nbsp;&nbsp;&nbsp;<a href="https://github.com/farhankabir12"><img src="https://image.flaticon.com/icons/png/512/25/25231.png" width="20" height="20"/></a>
3. Shadman Wadith (`Roll: AE-27`)&nbsp;&nbsp;&nbsp;<a href="https://github.com/wadith027"><img src="https://image.flaticon.com/icons/png/512/25/25231.png" width="20" height="20"/></a>&nbsp;&nbsp;&nbsp;<a href="mailto:wadith.24csedu.027@gmail.com"><img src="http://www.clker.com/cliparts/5/S/U/Y/A/R/email-icon-th.png" alt='Email Icon clip art' width="20" height="20"/></a>

## Repository and Workflow Description
The repository consists of two git submodules for the client and server respectively. Each repository is a self sufficient project. The client module is an Android Studio project and the server module is a Java gradle project (IntelliJ IDEA).

The git workflow follows the [Git Flow Workflow by Vincent Driessen](https://nvie.com/posts/a-successful-git-branching-model/).
It is based in two main branches with infinite lifetime.
- `master` — this branch contains production code. All development code is merged into master in sometime.
- `develop` — this branch contains pre-production code. When the features are finished then they are merged into develop.

During the development cycle, a variety of supporting branches are used:
- `feature-*` — feature branches are used to develop new features for the upcoming releases. May branch off from develop and must merge into develop.
- `hotfix-*` — hotfix branches are necessary to act immediately upon an undesired status of master. May branch off from master and must merge into master anddevelop.
- `release-*` — release branches support preparation of a new production release. They allow many minor bug to be fixed and preparation of meta-data for a release. May branch off from develop and must merge into master and develop.

## Video Demo
Goto [here](https://youtu.be/h0pA3SHEp_4).

## Download and Usage
To download and install/run goto the release pages for [hotkey-client](https://github.com/hoenchioma/hotkey-client/releases) (android client) and [hotkey-server](https://github.com/hoenchioma/hotkey-server/releases) (desktop client), and download the latest release.

(If you don't know how to install third party apks see [this](https://www.wikihow.tech/Install-APK-Files-on-Android))

Once installed, run the desktop client and press "Start" and then "QR code" button (this will show a QR code on the screen). Then with the app press "WiFI/LAN" (or Bluetooth depending on how you wish to connect) and scan the QR code. And voila the devices are connected.

## Support and Collaboration
If you wish to support or collaborate on this project please contact one of the members of the team.
