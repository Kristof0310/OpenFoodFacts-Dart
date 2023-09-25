<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://static.openfoodfacts.org/images/logos/off-logo-horizontal-dark.png?refresh_github_cache=1">
  <source media="(prefers-color-scheme: light)" srcset="https://static.openfoodfacts.org/images/logos/off-logo-horizontal-light.png?refresh_github_cache=1">
  <img height="48" src="https://static.openfoodfacts.org/images/logos/off-logo-horizontal-light.svg">
</picture>
<br>

## Smooth App: The new Open Food Facts mobile app for Android and iPhone

[![SmoothApp Post-Submit Tests](https://github.com/openfoodfacts/smooth-app/actions/workflows/postsubmit.yml/badge.svg)](https://github.com/openfoodfacts/smooth-app/actions/workflows/postsubmit.yml)
[![Create internal releases](https://github.com/openfoodfacts/smooth-app/actions/workflows/internal-release.yml/badge.svg)](https://github.com/openfoodfacts/smooth-app/actions/workflows/internal-release.yml)


## Code documentation

[Code documentation on GitHub pages](https://openfoodfacts.github.io/smooth-app/).


## Presentation

- This new mobile application aims to showcase Open Food Facts's power to a broad range of users through a smooth user experience and sleek user interface. It is a <b> Flutter application </b> by [Open Food Facts](https://github.com/openfoodfacts).
- We pioneered the collaborative scanning app in 2012. With this experimental app, we’re reinventing it from the ground up.
- Install it on **Android** ([Google Play](https://play.google.com/store/apps/details?id=org.openfoodfacts.scanner), [F-Droid](https://f-droid.org/fr/packages/openfoodfacts.github.scrachx.openfood/) or [Amazon App Store](https://www.amazon.com/Open-Food-Facts-food-Nutriscore/dp/B00U49IVIU)) or [iPhone/iPad](https://apps.apple.com/app/open-food-facts/id588797948). Note that a internal development build ([Android](https://play.google.com/apps/internaltest/4699092342921529278) or **iPhone/iPad** ([App Store](https://testflight.apple.com/join/c2tiBHgd)) if you'd like to use the results of your PRs quicker.

<img alt="app showcase" height='175' src="https://user-images.githubusercontent.com/1689815/168430524-3adc923a-1ce3-4233-9af5-02e9d49a76ca.png" align="left" hspace="1" vspace="1">

- Smooth-app is developed in parallel to the [openfoodfacts-dart](https://github.com/openfoodfacts/openfoodfacts-dart) plugin, which provides a high level interface with the Open Food Facts API and [openfoodfacts_flutter_lints](https://github.com/openfoodfacts/openfoodfacts_flutter_lints) which provides specific linting
- Every new interaction with the API should be implemented in the plugin in order to provide these new features to other developers.
- We support desktop platforms (Linux, macOS and Windows), but **only for development**

<br>

<details><summary><h2>Features of the app</h2></summary>

## Features

- a scan that truly matches who you are (Green: the product matches your criteria, Red: there is a problem, Gray: Help us answer you by photographing the products)
- a product page that's knowledgeable, building on the vast amount of food facts we collect collaboratively, and other sources of knowledge, to help you make better food decisions

## You can

- scan and compare in 15 seconds the 3 brands of tomato sauces left on the shelf, on your terms.
- get a tailored comparison of any food category
- set your preferences without ruining your privacy

## Criteria you can pick

- Environment: Eco-Score
- Health: Additives & Ultra processed foods, Salt, Allergens, Nutri-Score

</details>


## How to run the project

- Make sure you have installed flutter and all the requirements
  - [Official flutter installation guide](https://docs.flutter.dev/get-started/install)
- Currently, the app uses the previous version of Flutter (3.10). We plan to migrate soon.


We have predefined run configurations for Android Studio and Visual Studio Code

In order to run the application, make sure you are in the `packages/smooth_app` directory and run these commands:

- `flutter pub get .`

- On Android 🤖: `flutter run -t lib/entrypoints/android/main_google_play.dart`

- On iOS/macOS 🍎: `flutter run -t lib/entrypoints/ios/main_ios.dart`

- Troubleshooting🚀: If you get an error like `App depends on scanner shared from path which depends on camera_platform_interface from git, version solving failed.`  then run
  - `flutter pub cache clean` or manually delete  the  
  - `C:\Users\~\AppData\Local\Pub\Cache`  file.
 Then redo the above procedure to run the app.

- [Contributing Guidelines](https://github.com/openfoodfacts/smooth-app/blob/develop/CONTRIBUTING.md)

<br>
