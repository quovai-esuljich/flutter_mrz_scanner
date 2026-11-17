## 2.2.1-quovai.1

* Fix the Android preview rendering as a blank/white view (#15). The native
  view renders the camera preview into a nested `TextureView`, which
  Flutter's default `AndroidView` composition cannot capture into the
  composited frame. Render the `mrzscanner` platform view with full Hybrid
  Composition instead, which does support nested `TextureView` content.
* Quovai fork of 2.2.1 — carries only the fix above, without the 2.3.0 SDK
  constraint bump, so it still works on our pinned Flutter version.

## 2.2.1

* Fix Android 16KB Page size incompatibility by updating tesseract4android to 4.9.0 (by @khamidjon)

## 2.2.0

* Fix repository for 'io.fotoapparat:fotoapparat:2.7.0'
* Update example

## 2.1.1

* Add namespace (by @makhosi6)

## 2.1.0

* Support for Flutter 3.0.5 (by @dadagov125)

## 2.0.1

* Fix : Android crash (by @eusopht2021)

## 2.0.0

* Fix : iOS compiling errors for iOS 15 (by @gdaguin)
* Improvements : on Android, the camera is now focusing automatically (by @gdaguin)
* Port to null safety

## 1.0.0
* Android version redeveloped with Fotoapparat library
* Add overlay widget
* Flashlight on/off
* Take a photo

## 0.7.1

* Provide possibility to disable overlay

## 0.7.0

* First public version with basic iOS and Android scanners
