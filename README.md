
![Watchy face, featuring Wood Sitting on a Bed](GhostKittyWatchFace.jpg?raw=true "Wood Sitting on a Bed")
# Tiddies for Watchy

A watchface for [Watchy](https://watchy.sqfmi.com/) featuring NSFW images only you and your computer nerd friends from the mid-nineties will remember.

This fork of [Kitty for Watchy](https://github.com/MSGoodman/Kitty-for-Watchy) was written to add support for multiple static watchfaces, with individually positioned time and date fields, and provide the option to cycle between the watchfaces on an interval of your choosing. 

## Customization

### 24-Hour Clock or 12-Hour Clock

By default Tiddies for Watchy displays a 12-hour clock with a meridiem indicator (AM or PM). However, if you prefer a 24-hour clock you can change the value of `MILITARY_TIME` in `Ghost.cpp` to `true` and reupload this to your Watchy.

### Substituting your own image

If you'd like to swap out the picture of Ghost for one of your own it is very simple (instructions adapted from the [official Watchy guide](https://watchy.sqfmi.com/docs/create-watchface/)):

1. Crop your image to a 200px square
2. Use [image2cpp](http://javl.github.io/image2cpp/) to convert your image into a byte array
3. Replace the value of `ghostImage` in the file `image.h` with the byte array retrieved from step 2 

You may find that the locations of the text don't quite work with your image. If so, it is also easy to fix this by fiddling with the `OFFSET` `const`s at the top of `Ghost.cpp`.
