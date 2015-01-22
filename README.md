# Icon Sizerator - Apple App Store icon generator

This tool is a standalone service built in JavaScript on Node.js, which serves to assist iOS App creators in icon generation.

![](https://github.com/davidjpeacock/icon-sizerator/blob/master/icon-sizerator-ss.png)

Icon Sizerator is designed with throughput and low-cost in mind.  The backend image processing is performed by ImageMagick.

## Usage

You upload a source icon PNG of at least 1024x1024, and we'll instantly deliver a zip file filled with all the right sizes!  You can of course use the provided service at http://icon-sizerator.davidjpeacock.ca/

## Installation

If you wish to install this locally, you'll need to install ImageMagick through your preferred platform method.

* OS X: `brew install imagemagick`
* Ubuntu: `sudo apt-get install imagemagick libmagick++-dev libmagickcore-dev`

Then you can simply:

```
git clone https://github.com/davidjpeacock/icon-sizerator.git
cd icon-sizerator/
sudo npm install
node icon-sizerator.js
```

## Contributing

Contributions of issues and pull requests are most welcome.

## TODO

1. Auto-clean stale uploads/* folders; currently this is performed by a cron job, but this should occur natively within icon-sizerator.js  Or #2...
2. Alternatively a better solution would be to modify code to not need the on-disk folder, thus eliminating IO entirely.
3. Pretty up the upload form buttons; standard ones are ugly
