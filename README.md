# Realm-puzzle
A small puzzle game where players work to complete a jigsaw puzzle

# Overview
The Realm puzzle demo is a simple app that demonstrates a collaborative jigsaw puzzle sokving app.

# Installation

## Prerequisites

This app uses [Cocoapods](https://www.cocoapods.org) to set up the project's 3rd party dependencies. Installation can be directly (from instructions at the Cocapods site) or alternatively through a package management system like [Homebrew](brew.sh/).

### Realm Platform

This application demonstrates features of the [Realm Platform](http://lrealm.io) and needs to have a working instance of the Realm Object Server available to make tasks, and other data available between instances of the Puzzle app. The Realm Mobile Platform can be downloaded from [Realm  Platform](http://realm.io/pricing) and exists as a module server system that runs with nodejs and can be installed on macOS or Linux.  For information on installing the Realm Platform Server components, please download a copy of the [Developer edition](https://realm.io/pricing/).

### Realm Studio
Another useful tool is [Realm Studio](https://realm.io/products/realm-studio/) which is available for macOS, Linux nd Windows and allow developers to inspect and manage Realms. Realm Studio is recommended for all developers and can be downloaded from the [Realm web site](https://realm.io/products/realm-studio/).



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
