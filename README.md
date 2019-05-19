# MALM :octocat: <a href="https://travis-ci.org/BME-MIT-IET/MALM-iet-2019" target="_blank"><img src="https://travis-ci.org/BME-MIT-IET/MALM-iet-2019.svg?branch=master" alt="Travis build status" /> </a>
[Integration and Verification Techniques](http://www.mit.bme.hu/oktatas/targyak/vimiac04) course homework at BME MIT  
**Not the original GnuCash Android repository!**

## Bevezető, a projekt célja
A projekt célja a GnuCash nevű Androidos szoftver minőségének javítása különböző eszközökkel. Ezt két fő részben valósítjuk meg.  
👦 Matusek Márton - @matusekma   
👦 Putovits Ábel - @abelptvts  
👦 Zoltay Marcell - @MarcellZoltay  
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
  * Number of commits by time:![CommitByTime1](https://user-images.githubusercontent.com/25354615/57366672-ca4bce00-7187-11e9-9f24-0d59791b1bcb.PNG)
## Második feladatcsoport

A projekt második felében egységtesztek készítésével és kiegészítésével foglalkozunk a tesztek kódlefedettségének vizsgálatával párhuzamosan.

Task            |   Wiki            |  Issue         |  Branch         
:--------------:|:-----------------:|:--------------:|:-----------:
Kódlefedettség(Android Studio JUnit, JaCoCo, SonarCloud)       |      [Tesztek kódlefedettség mérése, tesztkészlet bővítése](https://github.com/BME-MIT-IET/MALM-iet-2019/wiki/Tesztek-k%C3%B3dlefedetts%C3%A9g%C3%A9nek-m%C3%A9r%C3%A9se-%C3%A9s-ez-alapj%C3%A1n-tesztk%C3%A9szlet-b%C5%91v%C3%ADt%C3%A9se) | [Tesztek kódlefedettségének mérése és reportolás integrálása a CI-ba](https://github.com/BME-MIT-IET/MALM-iet-2019/issues/7)| ✖️ 
Unit tesztek bővítése | ☝️ | [Kódlefedettség növelése](https://github.com/BME-MIT-IET/MALM-iet-2019/issues/8)|[test/unit](https://github.com/BME-MIT-IET/MALM-iet-2019/commits/test/unit)
Manuális tesztek |[Manuális tesztek készítése]( https://github.com/BME-MIT-IET/MALM-iet-2019/wiki/Manu%C3%A1lis-tesztek-k%C3%A9sz%C3%ADt%C3%A9se)|      ✖️         | ✖️

Coverage        |   Kiindulás         |  Elért         |  Különbözet         
:--------------:|:-------------------:|:--------------:|:-----------:
Package, Class  | 19,1%  (74/388)     |	20,6% (80/ 388) | +1,5% (+6/0)
Method          | 28,3%  (583/2 057)  | 30% (617/ 2057) | +1,7% (+34/0)
Line            | 26,2% (3 276/12 486)| 28,2% (3526/ 12486) | +2% (+250/0)

 *  ✔️ SonarCloud: [SonarCloud](https://sonarcloud.io/dashboard?id=malm-iet)
 *  ✔️ Travis CI build passing: https://travis-ci.org/BME-MIT-IET/MALM-iet-2019/branches
 *  ✔️ Merged to master:  2019.05.19. </br>
 * Number of commits by time:![image](https://user-images.githubusercontent.com/25354615/57989788-53c0a180-7aa0-11e9-8e1a-d71c86dfb5a9.png)

 
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
