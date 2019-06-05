# felica-reader

Code samples for reading FeliCa data on iOS 13.

![Demo](demo.gif)

## Build

Just build with Xcode 11.


Add system code to `com.apple.developer.nfc.readersession.felica.systemcodes` in Info.plist.
Each system code must be a discrete value. The wild card value (0xFF) isn't allowed.
Check [Apple Developer Documentation](https://developer.apple.com/documentation/bundleresources/information_property_list/systemcodes).

In this repository, the following system code has already been added.

- 0003: CJRC Standard (Suica, ICOCA, Kitaca, PASMO, TOICA, manaca, PiTaPa, SUGOCA, nimoca, HAYAKAKEN, RYUTO, SAPICA, odeca, KUMAMON's IC CARD, icsca, IruCa, PASPY, ...etc.)
- FE00: Student ID card by Japanese Univ. Co-op
