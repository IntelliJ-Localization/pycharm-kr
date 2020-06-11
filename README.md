This project is no longer maintained. Please use the official bundle: https://plugins.jetbrains.com/plugin/13711-korean-language-pack-eap 

[![Build Status](https://travis-ci.org/traff/pycharm-kr.svg?branch=master)](https://travis-ci.org/traff/pycharm-kr)

[![Coverage Status](https://coveralls.io/repos/github/traff/pycharm-kr/badge.svg?branch=master)](https://coveralls.io/github/traff/pycharm-kr?branch=master)


## How to build translation bundle

To build the resources_kr.jar bundle on Linux and macOs please run
```
./gradlew build
```

or on Windows

```
gradlew.bat build
```

The corresponding file will be created in build/libs

## How to use translation bundle

To use the translation bundle in PyCharm:

 * Copy build/libs/resources_kr.jar to $PYCHARM_HOME$/lib (where resource_en.jar is located).
 * Open or restart PyCharm.

 If your locale is Korean (ko_KR), then PyCharm will start with the UI translated to Korean.

*Note: not all UI strings are yet translated, so some strings may be still in English.*


![pycharm_kr.png](https://github.com/traff/pycharm-kr/blob/master/pycharm_kr.png "PyCharm in Korean")

## How to make a translation

To make a translation:
 * fork this repository
 * find strings to be translated in the *_ko_KR.properties files and change English text
to a corresponding Korean
 * to find strings that are to be translated you can use a [coverage report](https://coveralls.io/github/traff/pycharm-kr?branch=master)
 * commit changes
 * make pull-request

*Note: If an English string you want to translate is absent in _ko_KR.properties files, please create an issue.*

Let's make together a proper Korean localization of PyCharm!
