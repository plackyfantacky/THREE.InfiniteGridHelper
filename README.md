![InfiniteGridHelper-01](https://user-images.githubusercontent.com/28584767/157970587-bbcca0d6-7502-41fd-8a7b-fff087c36730.png)

# THREE.InfiniteGridHelper
Infinite anti-aliased grid.

[Original demo](https://codepen.io/Fyrestar/pen/wLxjYj) (you'll need to use an older version of ThreeJS for thi)

![InfiniteGridHelper](https://mevedia.com/share/InfiniteGridHelper.jpg)

2023 update by Plackyfantacky.

### Install and Usage

1. clone this repo or download the files into your project
2. in your main JavaScript file add the following near the top of your code:
```javascript
import InfiniteGridHelper from './THREE.InfiniteGridHelper/InfiniteGridHelper.js';
```
1. also add the following after your scene object is created:
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



