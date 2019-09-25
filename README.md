# Hotkey
A cross platform solution for controlling your PC from a mobile device
(This is a university project for the course CSE-2216 (Application Development Lab) at University of Dhaka.)

This project was mainly intentended as solution to a wide gap in applications that facilitate communication between mobile and desktop devices. Most existing applications cater to a specific needs. Our application aims to be a more general and cross platform solution for mobile desktop interaction, communication and control. 

It aims to facilitate ways to control and monitor various desktop functionalities (mouse, keyboard, media controls, etc.) from the mobile device. At the same time the desktop side application will be able to monitor some key information (notification, battery, etc.) of the mobile device. (Our focus at present is mostly on the prior, although it might change in the future)

## Planned Features

### Primary:
- Basic socket connection (over LAN)
- Mouse emulation
- Keyboard emulation
- Gamepad emulation
- Multimedia controls
- Slide presentation

### Secondary:
- Screen sharing
- Remote file managing (FTP server)
- Connection via PIN/QR code
- Over internet connection (not in same LAN)
- Terminal emulation (SSH)
- Custom shortcuts
- Link pushing and note saving
- Notification pushing (Bidirectional)

### Experimental:
- Wii like controller emulation
- Torrent pushing
- Gesture mouse
- Projector mode

NB. This is a rough outline of the planned features. For further detail and current progress please see the GitHub issues, projects and milestones.

## Members/Collaborators:
1. Raheeb Hassan (Roll: AE-42)
2. Farhan Kabir (Roll: AE-12)
3. Shadman Wadith (Roll: AE-27)

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
