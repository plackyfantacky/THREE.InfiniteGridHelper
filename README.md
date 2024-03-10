![InfiniteGridHelper-01](https://user-images.githubusercontent.com/28584767/157970587-bbcca0d6-7502-41fd-8a7b-fff087c36730.png)

# THREE.InfiniteGridHelper
Infinite anti-aliased grid.

> [Original demo](https://codepen.io/Fyrestar/pen/wLxjYj) (you'll need to use an older version of ThreeJS for this)

![InfiniteGridHelper](https://mevedia.com/share/InfiniteGridHelper.jpg)

### 2024 update by @plackyfantacky

Pretty much all credit/blame belongs to [Fyrestar](https://github.com/Fyrestar/THREE.InfiniteGridHelper). I just forked their work, updated it to work with more recent versions 
of ThreeJS and made it into an npm package for easy import. Nothing major.

### Install

```console
npm i @plackyfantacky/three.infinitegridhelper
```

### Usage

```javascript
import InfiniteGridHelper from 'InfiniteGridHelper';
```

Use it in your ThreeJS scene like this:

```javascript
// assuming you have already written...
// let scene = new THREE.Scene()

/* arguments are:
	- size1 (minor lines)
	- size2 (major lines)
	- color (must be a THREE.Color)
	- distance (default is 8000, but I find 30 'fades things out' nicely)
	- and axes
*/
let grid = new InfiniteGridHelper(0.1, 1, new THREE.Color('black'), 30, 'xzy');
scene.add(grid);
```

![InfiniteGridHelper-02](https://adamtrickett.com/Screenshot-2023-08-03.png)



