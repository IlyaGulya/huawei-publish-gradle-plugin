# 1.3.0

##### Add
* [issue#25](https://github.com/cianru/huawei-publish-gradle-plugin/issues/25):
Gradle 7.0 / Android Gradle Plugin 7.0 support
* add unit tests to automated github actions

# 1.2.4

##### Add
* Support of Gradle Portal and Gradle DSL..

##### Breaking changes
* Removed `clientId` and `clientSecret` plugin extension params as unsecured way for them setting.

##### Fix
* [issue#21](https://github.com/cianru/huawei-publish-gradle-plugin/issues/21):
App publication requires additional manual step to be available for users

# 1.2.2

##### Breaking changes
* If you are using AppBundle the current plugin version supports only Android Gradle Plugin v4.1.* due to
[AGP Issue](https://issuetracker.google.com/issues/109918868/). If you are using APK, then AGP version and Plugin version are irrelevant.

##### Fix
* [issue#11](https://github.com/cianru/huawei-publish-gradle-plugin/issues11): Handle Api Error for wrong `client_id` or `client_secret` values;
* [issue#16](https://github.com/cianru/huawei-publish-gradle-plugin/issues16): Plugin incorrectly detect AppBundle file location for AGP v4.1.*;

# 1.2.1

##### Add
* Support of release phases

##### Breaking changes
* Rename credentials parameter: `client_key` -> `client_secret`
* Replace `publish` plugin option on `deployType` one

##### Fix
* [issue#7](https://github.com/cianru/huawei-publish-gradle-plugin/issues/7):
AppBundle publication error: The file is being processed. It may take 2-5 minutes, depending on the size of the software package
* [issue#10](https://github.com/cianru/huawei-publish-gradle-plugin/issues/10):
Get error "call cds to query app information failed" for publishing with release phase

# 1.1.0

##### Add
* Support AppBundle
* Support system proxy
* Add CLI params for dynamically changes the plugin extension params

##### Fix
* [Issue#2](https://github.com/cianru/huawei-publish-gradle-plugin/issues/2):
Error on upload: 'The language does not exist!'

# 1.0.1

* Update dependencies: kotlin-1.3.72, gradle-6.6
* Added `publish` param to separate uploading and publishing a build file

# 1.0.0

* Support different Plugin settings for different buildTypes and flavors
* First release version

# 0.1.0

First released version. Support:
* Publish APK in Huawei AppGallery and submit it on all users after getting store approve

