##Change Log (2015/12/14):
* Android - Fix an issue with Video Callbacks returning false after a video had been watched

##Change Log (2015/10/16):
* Updated AdColony iOS to 2.6.0
  * Adds iOS 9 Support
* Updated AdColony Android to 2.3.0
* Remove two sample applications
* Reduce boilerplate
* Added a version property the AdColony object.
* iOS - Add PostProcessing

Special Notes
---
We've removed two of the Sample Applications from our examples. Moving forward we're focusing on a single high quality Sample Application that will best demonstrate using the AdColony Unity Framework.

We've also reintroduced PostBuildProcessor.cs for iOS. This works out of the box for Unity 5.X. This uses the (Unity Xcode API)[https://bitbucket.org/Unity-Technologies/xcodeapi]. For Unity 4.X it is still possible to take advantage of the Unity Xcode API. You'll need to follow the xcode api instructions for integrating with 4.X and Modify PostBuildProcessor.cs by removing the Unity5 preprocessor directives.

For iOS 9 is import to review the [iOS 9 integration guide](https://github.com/AdColony/AdColony-iOS-SDK/wiki/iOS-9)


##Change Log (2015/06/16):
* Android - Fixed an issue where OnVideoFinished was not being called

##Change Log (2015/06/04):
* Updated AdColony iOS to 2.5.1
* Updated AdColony Android to 2.2.2

##Change Log (2015/05/15):
* Android - Fixed an issue where callbacks were not being called after the video played

##Change Log (2015/05/13):
* iOS - Fixed an issue where changing orientations during video playback impacted the orientation of the application

##Change Log (2015/05/12):
* iOS - Fixed an issue where ads would return "false" to OnVideoFinished after they had shown

##Change Log (2015/04/27):
* Android - Fixed an issue where only the first ad would play under certain conditions

##Change Log (2015/04/20):
* Added Support for IAP Promo Adds

Special Notes
---
See the Wiki entries on OnVideoFinishedWithInfo

##Change Log (2015/02/23):
* CHANGELOG split from README
* Removed Support for Unity Pre4.3
* Simplified Samples directory
* Updated to AdColony iOS 2.5.0
* Updated to AdColony Andorid 2.2.1
* iOS - removed post processing

##Change Log (2014/11/06):
* iOS SDK 2.4.13 integrated

##Change Log (2014/07/23):
* A new build script has been created in order to facilitate automated integration when building for iOS, using the AdColony-Unity-SDK. This build script is called `AdColonyPostProcessBuild.cs'
  * This will now allow developers, who are targetting an iOS build, using the AdColony-Unity-SDK, to build and run automatically with-in Unity. The `AdColonyPostProcessBuild.cs` will handling linking the correct frameworks, and build settings needed for XCode to run
* With this new post process build script comes AdColony packages. These packages will be the new method in which developers can import the AdColony-Unity-SDK to their project
  * There are two packages now available, one for users who are still developing with Unity versions less than Unity 4.3, and one package for those who are developing for Unity versions greater than or equal to Unity 4.3
* New sample apps have been added, this is so that more clarity can be found when looking for example use cases
   * There is now a complex sample app that shows a suggested configuration that other developers might consider using when deciding how to implement their version of the AdColony-Unity-SDK. This is called the `AdColony AdManager`, but its file name is `ADCAdManager.cs`

##Change Log (2014/01/25):
* Android SDK 2.0.6 integrated
* Added `AndroidManifest_Unity43.xml` -- You must use this manifest if you are building with Unity 4.3.x, no change is necessary if you are using Unity 4.2.x and below

##Change Log (2013/11/26):
* iOS SDK 2.2.4 integrated
* Android SDK 2.0.4 integrated
* Public class methods `StatusForZone` exposed
* The `OnVideoFinished` delegate signature now includes a boolean parameter. The change requires a small update to existing integrations. For more information, consult the `Updating from Earlier Versions` section of the Unity SDK documentation for your platform (Android or iOS)
* `OnAdAvailabilityChange` delegate has been exposed

##Change Log (2013/09/23):
* iOS SDK 2.2.2 integrated
* Android SDK 2.0.3 integrated
* Public class methods `SetCustomID` and `GetCustomID` exposed
