
QuickMenuTemplate
=================

This is a template project for a main menu to help you get started building a Quick game.
It includes how to set up and tear down scenes, using the VirtualResolution helper,
saving and loading game state, simple music playback and examples for sprites and tweens.

This will become part of a full but compact game called "Condensation!", intended to
demonstrating more useful functionality like physics and more complex touch events.

The fule game is being added as part of the game jam template files here:
	https://github.com/marmalade/gbsgamejam


Features demonstrated
---------------------

Files:
  main.lua
  SceneGame.lua
  SceneMainMenu.lua
  Globals.lua  - Easy access global values
  helpers/...  - Utility classes, inc VirtualResolution from http://github.com/nickchops

The scenes demonstrate:
- setup
- teardown
- pre and post transition for setup and teardown
- removing nodes, disposing of any textures when leaving a scene to show resource
  management

main.lua:
- Includes utility classes
- Set's smart virtual resolution with user coords space set to iPhone 4 res

Menu scene:
- using nodes for subtrees to allow for easily moving things around the scene
- a background png
- buttons: start, high scores, sound on/off, exit - white sprites with colours applied and
  child text labels
- sound button turns music on/off
- play some music in background on loop
- a table storing scores and player info
- functions to save/load scores to file
- a high scores screen with
- enable/disable touch listeners
- tween animations with onComplete for button presses and switching menu
- suspend/resume
- use a transition when switching to game scene

Game scene:
- Just an empty scene skeleton that returns to the menu on touch

------------------------------------------------------------------------------------------
(C) 2014 Nick Smith.

All code is provided under the MIT license unless stated otherwise:

 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:

 The above copyright notice and this permission notice shall be included in
 all copies or substantial portions of the Software.

 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
