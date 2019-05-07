# MALM :octocat: <a href="https://travis-ci.org/BME-MIT-IET/MALM-iet-2019" target="_blank"><img src="https://travis-ci.org/BME-MIT-IET/MALM-iet-2019.svg?branch=master" alt="Travis build status" /> </a>
[Integration and Verification Techniques](http://www.mit.bme.hu/oktatas/targyak/vimiac04) course homework at BME MIT  
**Not the original GnuCash Android repository!**

## Bevezető, a projekt célja
A projekt célja a GnuCash nevű Androidos szoftver minőségének javítása különböző eszközökkel. Ezt két fő részben valósítjuk meg.  
👦 Matusek Márton - @matusekma   
👦 Putovits Ábel - @abelptvts  
👦 Zolty Marcell - @MarcellZoltay  
👦 Zahorán László - @zlacigit

## Első feladatcsoport

A szoftvert CI rendszerben üzemeljük be és statikus ellenőrzést végzünk el rajta. A statikus ellenőrzést is megpróbáljuk a CI build részévé tenni. A CI buildet a Travis eszköz segítségével végezzük. Statikus ellenőrzésre a SonarQube és a FindBugs eszközöket alkalmazzuk.

Task            |   Wiki            |  Issue         |  Branch         
:--------------:|:-----------------:|:-----------------:|:-----------------:
Travis CI     |[Travis CI beüzemelése](https://github.com/BME-MIT-IET/MALM-iet-2019/wiki/Travis-CI-be%C3%BCzemel%C3%A9se) | [Travis CI beüzemelése](https://github.com/BME-MIT-IET/MALM-iet-2019/issues/2) |[master](https://github.com/BME-MIT-IET/MALM-iet-2019/commits/master)
FindBugs      | [Statikus analízis FindBugs eszközzel](https://github.com/BME-MIT-IET/MALM-iet-2019/wiki/Statikus-anal%C3%ADzis-a-FindBugs-eszk%C3%B6zzel)  | [FindBugs analízis és javítás](https://github.com/BME-MIT-IET/MALM-iet-2019/issues/1)    | [fix/findbugs-fix](https://github.com/BME-MIT-IET/MALM-iet-2019/commits/fix/findbugs-fix)
SonarQube    | [Statikus analízis SonarQube eszközzel](https://github.com/BME-MIT-IET/MALM-iet-2019/wiki/Statikus-anal%C3%ADzis-SonarQube-eszk%C3%B6zzel)  | [SonarQube analízis és javítás](https://github.com/BME-MIT-IET/MALM-iet-2019/issues/3)   | [fix/sonarqube](https://github.com/BME-MIT-IET/MALM-iet-2019/commits/fix/sonarqube)

  * ✔️ Travis CI build passing: https://travis-ci.org/BME-MIT-IET/MALM-iet-2019/builds/528561407
  * ✔️ Merged to master:  2018.05.05. </br>
  * Number of commits by time:<img src="https://raw.githubusercontent.com/BME-MIT-IET/MALM-iet-2019/master/CommitByTime1.PNG" width="702" height="155" />

## Második feladatcsoport

A projekt második felében egységtesztek készítésével és kiegészítésével foglalkozunk a tesztek kódlefedettségének vizsgálatával párhuzamosan.

Task            |   Wiki            |  Issue         |  Branch         
:--------------:|:-----------------:|:--------------:|:-----------:
Feladat 1       |                   |                |
Feladat 2       |                   |                | 
 
 *  ❌ Travis CI build passing: 
 *  ❌ Merged to master:  Deadline: 2019.05.19. </br>
 
</br>

 **Original:**
 * Original project: https://github.com/codinguser/gnucash-android
 * Play Store: https://play.google.com/store/apps/details?id=org.gnucash.android&hl=hu
 * Original README.md below
</br>
</br>
</br>
</br>


# Introduction

GnuCash Android is a companion expense-tracker application for GnuCash (desktop) designed for Android.
It allows you to record transactions on-the-go and later import the data into GnuCash for the desktop.

Accounts            |  Transactions          |  Reports
:-------------------------:|:-------------------------:|:-------------------------:
![Accounts List](docs/images/v2.0.0_home.png)  |  ![Transactions List](docs/images/v2.0.0_transactions_list.png) |  ![Reports](docs/images/v2.0.0_reports.png)

The application supports Android 4.4 KitKat (API level 19) and above.

Features include:

  * An easy-to-use interface.

  * **Chart of Accounts**: A master account can have a hierarchy of detail accounts underneath it.  
    This allows similar account types (e.g. Cash, Bank, Stock) to be grouped into one master account (e.g. Assets).

  * **Split Transactions**: A single transaction can be split into several pieces to record taxes, fees, and other compound entries.

  * **Double Entry**: Every transaction must debit one account and credit another by an equal amount.
    This ensures that the "books balance": that the difference between income and outflow exactly
    equals the sum of all assets, be they bank, cash, stock or other.

  * **Income/Expense Account Types (Categories)**: These serve not only to categorize your cash flow, but when used properly with the double-entry feature, these can provide an accurate Profit&Loss statement.

  * **Scheduled Transactions**: GnuCash has the ability to automatically create and enter transactions.

  * **Export to GnuCash XML**, QIF or OFX. Also, scheduled exports to 3rd-party sync services like DropBox and Google Drive

  * **Reports**: View summary of transactions (income and expenses) as pie/bar/line charts


# Installation

There are different ways to get the GnuCash app for Android; through
the app store, from github or building it yourself.


### App Store

<a href="http://play.google.com/store/apps/details?id=org.gnucash.android">
  <img alt="Android app on Google Play" src="http://developer.android.com/images/brand/en_generic_rgb_wo_60.png" />
</a>

### From GitHub

Download the .apk from https://github.com/codinguser/gnucash-android/releases

## Building

### With Gradle

This project requires the [Android SDK](http://developer.android.com/sdk/index.html)
to be installed in your development environment. In addition you'll need to set
the `ANDROID_HOME` environment variable to the location of your SDK. For example:

    export ANDROID_HOME=/home/<user>/tools/android-sdk

After satisfying those requirements, the build is pretty simple:

* Run `./gradlew build installDevelopmentDebug` from the within the project folder.
It will build the project for you and install it to the connected Android device or running emulator.

The app is configured to allow you to install a development and production version in parallel on your device.

### With Android Studio
The easiest way to build is to install [Android Studio](https://developer.android.com/sdk/index.html) v2.+
with [Gradle](https://www.gradle.org/) v3.4.1
Once installed, then you can import the project into Android Studio:

1. Open `File`
2. Import Project
3. Select `build.gradle` under the project directory
4. Click `OK`

Then, Gradle will do everything for you.

## Support

Google+ Community: https://plus.google.com/communities/104728406764752407046

## Contributing

There are several ways you could contribute to the development.

* Pull requests are always welcome! You could contribute code by fixing bugs, adding new features or automated tests. 
Take a look at the [bug tracker](https://github.com/codinguser/gnucash-android/issues?state=open)
for ideas where to start. It is also preferable to target issues in the current [milestone](https://github.com/codinguser/gnucash-android/milestones). 
* Make sure to read our [contribution guidelines](https://github.com/codinguser/gnucash-android/blob/master/.github/CONTRIBUTING.md) before starting to code. 

* Another way to contribute is by providing translations for languages, or improving translations.
Please visit [CrowdIn](https://crowdin.com/project/gnucash-android) in order to update and create new translations

For development, it is recommended to use the Android Studio for development which is available for free.
Import the project into the IDE using the build.gradle file. The IDE will resolve dependencies automatically.

# Licence
GnuCash Android is free software; you can redistribute it and/or
modify it under the terms of the Apache license, version 2.0.
You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

# IVT Spaceship

This is a sample application for the [Integration and Verification Techniques](http://www.mit.bme.hu/oktatas/targyak/vimiac04) course at BME MIT.

The application is simplified and deliberately contains bugs.

## Getting started

- The project is implemented in Java 8.
- The project can be built using [Maven](https://maven.apache.org/).
- [JUnit](http://junit.org/junit4/) is used for tests, and [Mockito](http://site.mockito.org/) for isolating dependencies.

Clone the repository and execute Maven to build the application:

```
mvn compile
```

To compile and run tests also execute:

```
mvn test
```

(That will be enough to know for the current exercises. If you are more interested, see [this](https://github.com/FTSRG/swsv-labs/wiki/0b-Build-tools) short guide about Maven.)

As this is a really simple project, you can use the command-line build tool and a light-weight IDE like the [Atom](https://atom.io/) editor. Just be sure to enable collapsing directories (_File / Settings / Packages / tree-view / Collapse directories_).

## Overview++EditedBy Branch-A;++EditedBy Branch-B Conflict Solved

The project represents an alpha version of a spaceship.

- The ship (`SpaceShip` interface) can fire one or more lasers or torpedos.
- We have only one spaceship as of now (`GT4500`).
- Currently two firing modes (`FiringMode`) are supported: firing only one or all instances of a given weapon type.
- Lasers are not yet implemented, but the code for torpedo stores are ready (`TorpedoStore`).
- For the GT4500 ship the rules for firing torpedoes can be found in the Javadoc comment of method `fireTorpedos`. They are already partially implemented.
- There are currently two tests (`GT4500Test`), but be aware that they are not proper unit tests, as they do not isolate the dependencies of the tested class.
++EditByMe
