ℹ️ 日本の NFC カードを読み取るためのライブラリを開発、公開しています。 ℹ️

[treastrain/TRETJapanNFCReader](https://github.com/treastrain/TRETJapanNFCReader)
日本の NFC、FeliCa カード向けリーダーライブラリ（iOS 13.0 以降）

# felica-reader

![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)

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
