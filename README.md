# Simplenuff Chess

Chess game based on "[The Kilobyte's Gambit](https://vole.wtf/kilobytes-gambit/)" with a couple of new features: undo and choose color to play. Original [nanochess engine](https://nanochess.org/) by Oscar Toledo. Graphics by [Pinot](https://www.instagram.com/pinot/). Used with kind permission of the original authors I could contact with.

[PLAY NOW](https://gallargit.github.io/SimplenuffChess/)

# About
I got to know this game and I liked playing with it. Since I'm not a very good chess player I often got frustrated when I made a silly move in the middle of the game spoiling it. So I started tweaking the code around to figure out a way to implement an "Undo" button. Then this feature became a full "History Undo", and then I thought... well, why not implement play as black as well?

Since I spent quite some time doing this I thought it would be a good idea to release as open source, so here it is.

# New features
- Undo feature
- Play as black or white feature
- New colors for the chess pieces
- Removed animations, help screens, etc... Simplenuff!!!

# Querystring switches
- calcdepth: it will change the calculation depth the engine uses. Values range from 2 to 7. Default is 3. The bigger the number, the slower it gets. Any number above 4 will make it really slow.
`index.html?calcdepth=4`

- playasblack: it will make the player play as black.
`index.html?playasblack=1`

you can combine both
`index.html?playasblack=1&calcdepth=3`

# Technical info
Everything I modified is included in the "index.html" file. My modifications are usually written in capital letters, so that it can be easy to find what's new.

# Known Bugs
- Castling does not work for black, I could not figure out how to make it work yet. I noticed you can castle with queen's knight if playing as black. Some bit is out of place somewhere. Oscar Toledo told me to invert the board before moving and then invert it again to make it work, but whenever doing that everything worked horribly wrong.

- Animation sometimes does not work as usual after undoing. Just a minor glitch.
