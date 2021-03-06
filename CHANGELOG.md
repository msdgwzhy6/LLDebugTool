## [1.1.0](https://github.com/HDB-Li/LLDebugTool/releases/tag/1.1.0) (06/07/2018)

### Add screenshot function.

Increases the need to the permissions of the album, but it is not necessary, if the project has the authority, save will be synchronized to photo album, if the project doesn't have the permission, is saved into the sandbox alone, LLDebugTool will not actively apply for album permissions.

<div align="left">
<img src="https://raw.githubusercontent.com/HDB-Li/HDBImageRepository/master/LLDebugTool/ScreenGif-Screenshot.gif" width="20%"></img>
</div>

#### Add

* Add `LLScreenshotHelper` in `Helper` folder, used to control screenshot.
* Add `LLScreenshotView` folder in `UserInterface/Others` folder, used to show and draw screenshot.
* Add `LLDebugToolMacros.h`, used to manage public macros.

#### Update

* Update `LLBaseNavigationController` and `LLBaseViewController` to repair toolbar's frame is wrong when hiding tabbar.
* Update `LLAppHelper` to fix iPhone X getting network status error.
* Remove `LLog` macros in `LLDebugTool.h` and moved to `LLDebugToolMacros.h`

#### Additional Changes

* Update demo for saving screenshots to photo albums when screenshots are taken.

## [1.0.3](https://github.com/HDB-Li/LLDebugTool/releases/tag/1.0.3) (05/31/2018)

Fix some leaks.

#### Update

* Call `CFRelease` in `LLAppHelper`.
* Resolve circular references caused by the `NSURLSessionDelegate` in `LLURLProtocol`.
* Call `Free` in `LLBaseModel`.
* Fix analyze warning in `LLBaseViewController` / `LLFilterOtherView`.
* Uncoupled code in `LLTool` / `LLNetworkContentVC`.

#### Additional Changes

* Add `NetTool`(Use URLSession in a singleton.) and update `ViewController` (Fix a circular reference.)

## [1.0.2](https://github.com/HDB-Li/LLDebugTool/releases/tag/1.0.2) (05/21/2018)

* Fix the side gesture recognizer bug when pop.

## [1.0.1](https://github.com/HDB-Li/LLDebugTool/releases/tag/1.0.1) (05/12/2018)

* Support iOS8+.

## [1.0.0](https://github.com/HDB-Li/LLDebugTool/releases/tag/1.0.0) (05/09/2018)

* Initial release version.
* Contains the following functions:
  
  * Monitoring network requests.
  * Save and view log information.
  * Crash information collection.
  * Monitoring app properties.
  * Operation of sandbox file.
  
