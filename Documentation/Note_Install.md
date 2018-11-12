# Metal city
### path:
    D:\Repository\Pierre56\Metal city

## Install CLI tools

To build scenes for Decentraland you will need to install the Command Line Interface (CLI).
The CLI allows you to compile and preview your scene in an “off-chain” development environment.

## Install de [Node](Metal city\Node\Notes Node Install)
### Path
    D:\Program files\Node

## Intall de [Python 2.7](https://www.python.org/downloads/)
### Path
    D:\Program files\go-ipfs\ipfs.exe

## Intall de [IPFS](https://ipfs.io/)

go-ipfs is the main implementation of IPFS. It includes: - an IPFS core implementation - an IPFS daemon server - extensive command line tooling - an HTTP API for controlling the node - an HTTP Gateway for serving content to HTTP browsers

### Path
    D:\Program files\go-ipfs\ipfs.exe


## Commandes exécutées as admin pour Install

    cd D:\Repository\Pierre56\Metal city

    npm install --global --production windows-build-tools

    npm install -g decentraland

    npm update -g decentraland

-----
    mkdir Scene
>(pour contenir scene par defaut)

    dcl init
> Success! Run 'dcl start' to see your scene
> Edit "parcels" property at scene.json to make your scene fit your estate.
> The dcl init command creates a Decentraland project in your current working directory containing a scene.

### Problèmes rencontrés

#### 1. Could not install Visual Studio Build Tools.
Please find more details in the log files, which can be found at
C:\Users\pierre le dorze\.windows-build-tools

Maj de Visual Studio Community 2017
Maj Visual Studio Build Tools


## Visualisation de la scene

https://docs.decentraland.org/development-guide/scene-files/


    dcl start

[URL preview = 172.17.0.73:8000](http://172.17.0.73:8000)


## Local scenes include the following files:

* scene.tsx: The entry point of the scene.
* scene.json: The manifest that contains metadata for the scene.
* package.json and package-lock.json: Specify the versions of all dependencies of the scene.
* build.json: The file with the instructions to build the scene.
* tsconfig.json: Typescript configuration file.


## Recommended file locations#
when you deploy your scene to Decentraland, any assets or external libraries that are needed to use your scene must be either packaged inside the scene folder or available via a remote server.

We suggest using these folder names consistently for storing the different types of assets that your scene might need:

* 3d models: /models
* Videos: /videos
* Sound files: /sounds
* Image files for textures: /materials
* .tsx definitions for reusable components /components
