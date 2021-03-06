# Bing Maps SDK for iOS

Version 1.0.0 - September 2019
==============================
## Breaking changes
- Updates various public classes.
- Introduces `MSGeoshape` and `MSGeoposition` classes, and refactors all `MSGeo` classes accordingly.
- Renames `MSGeolocation` to `MSGeopoint`.
- Renames several `MSMapView` methods and properties.
- Renames various callback interfaces and ensures callbacks are invoked on the UI thread.
- Renames several `MSMapFlyout` methods and properties.
- Renames several `MSMapUserInterfaceOptions` properties.
- Renames a few `Search` types and callback interfaces.
- Moves all `Search` enums into their own files.

For more details see the full list of [Breaking API changes in version 1.0](https://docs.microsoft.com/en-us/bingmaps/sdk-native/v1-breaking-changes/).

## Improvements
- Improves load time by over 30%.
- Includes optimizations for vector map render mode.
- Adds `MSGeoposition` and `MSGeopoint` convenience constructors for `CLLocationCoordinate2D` and `CLLocation`.
- Adds support for complex polygons.
- Adds support for custom flyout views.
- Adds support for language and region settings in Map Services.
- Reduces universal framework size by removing specific `armv7s` architecture binary from the framework.
## Resolved Issues
- Enables bitcode.
- Fixes issues that prevented apps from publishing to the Store.
- Fixes a memory leak on map dispose.
- Fixes a race condition that prevented map content from loading.
- Fixes resolution issues reported in some devices.
- Fixes Thread Checker warnings.

Version 0.2.0 - July 2019
=========================
## Breaking changes
- Renames enum `MSMapCameraChangeCause` to `MSMapCameraChangeReason`.
## Improvements
- Adds default values for `MSMapFlyout` properties `PlacementOffset` and `ZIndex`.
## Resolved Issues
- Fixes a crash caused by calling `MSMapIcon::isFlyoutVisible` when flyout does not exist.

Version 0.1.4 - June 2019
=========================
## Resolved Issues
- Fixes a crash on map dispose.

Version 0.1.3 - June 2019
=========================
## Improvements
- Improves pan gesture.
## Resolved Issues
- Fixes unexpected map movements after rotation and stretch & pinch gestures.

Version 0.1.2 - May 2019
========================
## Improvements
- Improves default set scene animations.
- Includes optimizations for raster map render mode.
## Resolved Issues
- Fixes a few race conditions.
- Fixes incorrect status code for reverse geocoding.
- Fixes a styling issue in raster map render mode.

Version 0.1.1 - May 2019
========================
## Resolved Issues
- Fixes a crash in Map Services.

Version 0.1.0 - May 2019
========================
Initial release of the Bing Maps SDK for iOS (developer preview).

Features a native map control and an accompanying map services API set.
The map control is powered by a full vector 3D map engine with a number of
standard mapping capabilities, including displaying icons, drawing polylines
and polygons, and overlaying texture sources.
