# ZMK Config

This repo stores keymaps for my keyboards running on ZMK.

It enables building custom keymaps without having to go through the process of installing the ZMK / Zephyr toolchain which can be quite painful.

## To Use
- Fork this repo
- In your fork, click on the "actions" tab and enable GitHub actions
- Clone the repo to your machine
- Checkout the branch which you want to build, see below for options `git checkout <branch>`
- Edit the keymap to customise as required, and save once done
- Add the modified file to git `git add .`
- Commit the changes `git commit -m "update keymap"`
- Push the changes `git push`
- With the above done, head to your fork, select actions, and click on the latest build run. When it finishes, there will be an artifact called "firmware" you can download.

## Available Keymaps / Branches
### Chalice
- `chalice_nn2_default` Suggested layout for Chalice, running on a nice!nano v2
- `chalice_nn_default` Suggested layout for Chalice, running on a nice!nano
- `chalice_nn2_splitbs` Suggested split backspace layout for Chalice, running on a nice!nano v2
- `chalice_nn2_josh` A Colemak layout with dedicated function and RGB layers, built for a n!n v2
- `chalice_nn_josh` A Colemak layout with dedicated function and RGB layers, built for a n!n

### Entropy
- `entropy_josh` Colemak layout with split spacebar, numpad, and encoder support. 

## Making your own keymap / branch
- First checkout the most similar branch to what you want (e.g. n!n or n!n v2, QWERTY vs Colemak) `git checkout <branch>`
- Create a new branch based on currently checked out branch `git checkout -b <your-branch-name>`
- Then follow the above instructions to modify and commit / push your changes to GitHub, where the keymap will then be built.