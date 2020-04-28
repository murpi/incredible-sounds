Your Very Own Soundboard
========================

A simple soundboard designed to play any sound you want on command.

Click `Show` in the header to see your app live. Updates to your code will update live.

The Files
---------

### ← README.md

That's this file, where you can tell people what your cool website does and how you built it.

### ← index.html

This is where most of the work happens! 

### ← style.css

CSS files add styling rules to your content to make it look pretty.

### ← assets

Drag in `assets` -- in this case audio samples, to add them to your project.

Remixing Your Soundboard
------------------------

To make your own sound-board, use Glitch's `Remix` button to create a new project. From there, it's pretty straight forward:

1. Use the assets folder to upload your audio.
2. Link those assets in corresponding order in the `<audio>` tag within `index.html` file, like this:
```<audio id="sound1" src="YOUR ASSET LINK GOES HERE" preload="auto"></audio>```
It will support mp3, mp4, wav, and more.
3. Rename each button's display name:
```<button onclick="document.getElementById('sound1').play()" class="sound-pad 1">DISPLAY NAME</button>```

Adding More Sounds
------------------
To add even more pads + sounds, add copies of the following lines to the bottom of each section:

Your audio file:

```<audio id="SOUNDNUMBER" src="YOUR ASSET LINK GOES HERE" preload="auto"></audio>```

The button/pad:

```<button onclick="document.getElementById('SOUNDNUMBER').play()" class="sound-pad SOUNDNUMBER">DISPLAY NAME</button>```

The key binding, if you want to add more keyboard shortcuts:

```
Mousetrap.bind('LETTER', function(e) {
      document.getElementById('SOUNDNUMBER').play()
    });
```

Need some help finding good sounds? Check out [CreativeCommons](https://creativecommons.org/about/program-areas/arts-culture/arts-culture-resources/legalmusicforremixing/) for some good, royalty-free sample ideas. Or, use your phone's audio notes app to record sounds all around you!


### Made with [Glitch](https://glitch.com/) by [Ezra Mechaber](http://ezramechaber.glitch.me). Cover art by [Musketon](https://www.musketon.com/).


\ ゜o゜)ノ
