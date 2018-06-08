# svgr-watch-file-test

Quick example how to generate React components from SVG files on the fly by watching a directory, and only recompiling changed files.

    npm run watch
    
This will create a `.js` file with a react component in a `./js`directory for each `.svg` file in `./svg` directory ONCE and then watch `./svg` for changes. When an `.svg` file is being changed or added, the corresponding `.js` file will be built.

*TODO*
* massage to path/ only pass the filename instead of path to `svgr` to avoid creating an `svg` subdirectory in `js`
* delete corresponding `js`file once `svg`file is deleted