# rendr-demo


## Installation
```bash
$ npm install akileez\rendr-demo
```

## Usage

See index.js for the configuration object.

```js
var rendr = require('rendr')
var config = {
  defaults: {
    //...
  },
  
  globals: {
    // handlebars contextual stuff can go here
  }
}

rendr(config)
```

## Directory Structure

This is the base directory structure I used when developing `rendr`. You should be able to alter as you see
fit but something will probably catch a snag. There are some hardcoded items within due to me only thinking
of myself. I did not test any alternative structres yet. This project was only an experiment to see if I could do it.

```bash
❯ tree -d -L 2 -I node_modules
.
├── assets (staging area)
│   ├── css
│   ├── fonts
│   ├── ico
│   ├── img
│   ├── js
│   └── pdf
├── build (build directory. Not needed. Will be created at rendr time.)
│   ├── articles
│   └── assets
├── config (handlebars contextual data. app for sitewide, data for specific purposes)
│   ├── app
│   └── data
├── helpers (your handlebars helpers)
├── layouts (how I structure projects)
│   ├── globals (global layouts)
│   ├── regions (sub-layouts filter into the global -- used to structure individual pages/templates)
│   ├── sectors (were I keep partials. I only use partials for the layouts.)
│   └── templates (page templates. I structure a site within this folder)
├── pages (you could call these partials but they are individual modules used to fill in templates
    structure this as you see fit.)
├── scripts (javascript files. rendr extensions dependent on structure here. styles and support included)
│   ├── bootstrap
│   ├── dev
│   ├── libs
│   ├── plugins
│   ├── theme
│   └── views
├── styles (less files)
│   ├── bootstrap
│   ├── development
│   ├── theme
│   └── vendor
└── support (static assests ... like bower)
    ├── fonts
    ├── img
    ├── js
    ├── pdf
    └── php

38 directories
```

## Why?


## See Also
-

## License
[ISC](https://github.com/akileez/rendr-demo/blob/master/LICENSE)

