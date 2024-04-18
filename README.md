# ldraw-parts-library
Upload of the LDraw parts library intended to be used for static file loading in github examples.

Parts library downloaded from [here](https://library.ldraw.org/updates?latest) and unofficial parts from [here](https://library.ldraw.org/tracker) on January 30th, 2023.

color definitions downloaded from [here](https://www.ldraw.org/article/547.html) on May 15th, 2023.

# Use with three.js LDrawLoader

```js
const loader = new LDrawLoader();
loader.setPartsLibraryPath( 'https://raw.githubusercontent.com/gkjohnson/ldraw-parts-library/master/complete/ldraw/' );
await loader.preloadMaterials( 'https://raw.githubusercontent.com/gkjohnson/ldraw-parts-library/master/colors/ldcfgalt.ldr' );

loader.load( 'https://raw.githubusercontent.com/gkjohnson/ldraw-parts-library/master/complete/ldraw/10030-1%20-%20Imperial%20Star%20Destroyer%20-%20UCS.mpd' );
```
