# balena-MagicMirror
This projects combines the [MagicMirror²](https://github.com/MichMich/MagicMirror) project with the [balenaCloud](balena-cloud.com) platform.

## How to install
+ Clone this repository
+ Initialize the submodules
    + execute `git submodule update --init --recursive`
    
## Add your config.js
The `config.js` file defines the content of your MagicMirror. Modify the existing `config.js` file in `MagicMirror/config` as you like.

## Add modules
Modules must be placed in the `MagicMirror/modules`. You can use git submodules or just copy the module into this directory. 

## Upload to your project
+ Install the `balena` CLI tools and push to your project
    + `balena push MY_PROJECT`
+ Add the enviromental variable `WPE_URL` with the IP and port of your MagicMirror project to display the interface on the `balena-wpe` browser.

## Known issues
- [ ] Unstable MagicMirror service (restarting every now and then)
- [ ] browser starting before the MagicMirror service has been starting resulting in a white screen 