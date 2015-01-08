# Ember-cli-imagemin

Minify images with imagemin. This addon is a thin wrapper around [broccoli-imagemin](https://github.com/Xulai/broccoli-imagemin).


## Installation

    npm install ember-cli-imagemin --save-dev


## Options

### Broccoli Imagemin options

Define options to be passed directly to `broccoli-imagemin`.

    var app = new EmberApp({
      imagemin: {
        interlaced: true,
        optimizationLevel: 3,
        progressive: true,
        lossyPNG: false
      }
    });

Read more about the options you may pass in on the [broccoli-imagemin](https://github.com/Xulai/broccoli-imagemin) page.

### Enabled

Type: `Boolean`  
Default: `app.env === 'production'`

Enable minification of images. Defaults to `true` in production environment, otherwise `false`.

    var app = new EmberApp({
      imagemin: {
        enabled: true
      }
    });

Alternatively, you may simply set `{ imagemin: true }` as a shortcut.