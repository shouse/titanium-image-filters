# Titanium Image Filters

Use the GPUImage library to apply pre-built and custom filters to images in Titanium Edit
Add topics.

## Credits

Really all credits of this module should go to [@BradLarson](https://github.com/BradLarson) who made the
amazing [GPUImage](https://github.com/BradLarson/GPUImage) library! There are over [125 built-in filters](https://github.com/BradLarson/GPUImage#built-in-filters)
plus the ability to create own filters via shaders.

## Features

Right now, this module only supports applying built-in filters to a still image:
```js
var GPUImage = require('ti.gpuimage');
var image = GPUImage.filteredImage({
  image: 'myImage.png',
  filter: GPUImage.FILTER_SEPIA // or the filter class name, e.g. `GPUImageHueFilter`
});
```
You cannot specify filter properies by now, so I am thinking about moving the filter to
an own class that does KVO to check and supply the used properties dynamically.

## Android

I created an Android module project as well, which does nothing right now, but could use [this library](https://github.com/CyberAgent/android-gpuimage).
Go ahead!