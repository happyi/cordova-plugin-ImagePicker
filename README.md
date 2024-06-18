cordova-imagePicker
===================
forked from giantss/cordova-plugin-ImagePicker

support android 10

## Installing the plugin

```
cordova plugin add cordova-plugin-mz-imagepicker
```

## Using the plugin

The plugin creates the object `window.imagePicker` with the method `getPictures(success, fail, options)`

Example - Get Full Size Images (all default options):
```javascript
window.imagePicker.getPictures(
	function(results) {
		for (var i = 0; i < results.length; i++) {
			console.log('Image URI: ' + results[i]);
		}
	}, function (error) {
		console.log('Error: ' + error);
	}
);
