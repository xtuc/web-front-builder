# Web-front-builder

Docker toolbox for compiling a web front-end, which includes:
* [Node.js](https://nodejs.org/) - Node.js
* [Npmjs](npmjs.com) - Npmjs
* [Bower](http://bower.io) - Bower
* [Grunt](http://gruntjs.com) - Grunt
* [Gulp](http://gulpjs.com) - Gulp
* [Less](http://lesscss.org) - Less
* [Typescript](http://www.typescriptlang.org/) - Typescript

### Usage

You need first to set the directory you want to build. For exemple the current dir :
```sh
WORK_DIR=$(pwd)
```

###### npm dependencies:
```sh
docker run -v $WORK_DIR:/root xtuc/web-front-builder npm install
```

###### bower dependencies:
```sh
docker run -v $WORK_DIR:/root xtuc/web-front-builder bower install --allow-root
```

###### grunt tasks:
```sh
docker run -v $WORK_DIR:/root xtuc/web-front-builder grunt
```

###### gulp tasks:
```sh
docker run -v $WORK_DIR:/root xtuc/web-front-builder gulp
```

License
----

MIT
