# GPX-Googlefit 

a [Sails](http://sailsjs.org) application that imports GPX files to GoogleFit. By no means complete, but will allow one to take a workout exported to GPX, and drag/drop for import to [Google Fit](https://fit.google.com/).

1. `npm install`
1. (`npm install -g bower ` if you don't have it)
2. `bower install` 
3. add your [Google oauth creds](https://console.developers.google.com) to `config/env/development.js` or production
3. `sails lift` or you can run a script like `./scripts/debug.sh`
4. navigate to `http://localhost:1337`
5. authorize the application to use your google account
5. drag/drop your `gpx` files at will


###I only have `.tcx` files.
I had the same problem...

`./gpsbabel/src/batch.sh` - follow the prompts

you can read more about the gpsbabel helper in the [gpsbabel/README](./gpsbabel/README.md) file.

#TODOs
1. better calculation for calories
2. implement heartrate from `tcx` files
