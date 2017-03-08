# Realm-puzzle
A small puzzle game where players work to complete a jigsaw puzzle

# Overview
The Realm puzzle demo is a simple app that demonstrates a collaborative jigsaw puzzle sokving app.

# Installation

## Prerequisites

This app uses [Cocoapods](https://www.cocoapods.org) to set up the project's 3rd party dependencies. Installation can be directly (from instructions at the Cocapods site) or alternatively through a package management system like [Homebrew](brew.sh/).

### Realm Mobile Platform

This application demonstrates features of the [Realm Mobile Platform](http://lrealm.io) and needs to have a working instance of the Realm Object Server available to make tasks, and other data available between instances of the Fieldwork app. The Realm Mobile Platform can be downloaded from [Realm Mobile Platform](http://realm.io) and exists in two forms, a ready-to-run macOS version of the server, and a Linux version that runs on RHEL/CentOS versions 6/7 and Ubuntu as well as several Amazon AMIs and Digital Ocean Droplets. The macOS version can be run with the Fieldwork right out of the box; the Linux version will require access to a Linux server.


### 3rd Party Modules

The following modules will be installed as part of the CocoaPods setup:

- [Realm](https://realm.io)  The main line Realm bindings for Cocoa/ObjC
- [RealmSwift](https://realm.io)  The Realm bindings for Cocoa/Swift
- [Realm LoginKit](https://github.com/realm-demos/realm-loginkit) A Realm control for logging in to Realm servers


## Preparing the Realm Object Server

The app is meant to be played by 2 players each of who connect to the same Realm Object Server which acts as a rendezvous service for info about the movement of the puzzle pieces o each user's device.

The Realm puzzle application can be used with any version of the Realm Object Server (Developer, Professional or Enterprise).  No special permissions are required - each user simply logs in to the shared server and the game play begins.


## Puzzle Views
The Realm Puzzle consists of two screens: the login view and the puzzle view:

The login view allows each user to log into a shared Realm object server that will server as a rendezvous point.
<center> <img src="/Graphics/realm-puzzle-login.png" width="512" height="384" /><br/>Login</center><br>

The puzzle view itself is where the game is placed.  At startup the puzzle is randomized and the positions of the pieces are distributed to each player.

<center> <img src="/Graphics/realm-puzzle-main.png" width="512" height="384" /><br/>Main Puzzle View</center><br>

Gameplay continues until the puzzle is solved.

# Realm Object Server Features

@TODO: __Describe how Puzzle uses ROS to keep the players in sync__

# License

The Realm Puzzle is distributed under the terms of the  [MIT License](https://en.wikipedia.org/wiki/MIT_License)
