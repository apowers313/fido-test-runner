# FIDO Testing Framework

This is a generic framework for testing all flavors of FIDO stuff.

## How to use

* Clone this repo
* Change directories to the root of the repo
* Start a server: `python -m SimpleHTTPServer 8000` (or similar)
* Connect to the server through your favorite server: [http://localhost:8000](http://localhost:8000)
* Click on the test you want to run
* Change code to fix failing tests
* [ ... repeat ... ]
* When your code passes, click "submit" to submit your results to FIDO

## Supported Platforms

* Any browser: run the tests with the instructions above
* Android: download [Android Cordova](https://cordova.apache.org/docs/en/latest/guide/platforms/android/) platform (not yet written)
* iOS: download [iOS Cordova](https://cordova.apache.org/docs/en/latest/) platform (not yet written)
* Windows: download [Windows Cordova](https://cordova.apache.org/docs/en/latest/guide/platforms/win8/) platform (not yet written)
* OSX: download [OSX Cordova](https://cordova.apache.org/docs/en/latest/guide/platforms/osx/) platform (not yet written)

## External Authenticators 

* USB: download [USB Proxy]() (not yet written)
* NFC: download [NFC Proxy]() (not yet written)
* BLE: download [BLE Proxy]() (not yet written)

## How this code is organized

* README.md - this file
* index.html - list of available test suites
* test-runner.html - the main test runner
* *-testlist.json - lists of tests to be run for each test suite
  * test/* - test implementations
  * helper/* - helper libraries for tests
  * lib/* - third-party libraries for tests
  * css/* - CSS files for browser UI
