# KDEDateLabel
[![Build Status](https://travis-ci.org/delannoyk/KDEDateLabel.svg)](https://travis-ci.org/delannoyk/KDEDateLabel)
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)
![CocoaPods Compatible](https://img.shields.io/cocoapods/v/KDEDateLabel.svg)
![Platform iOS](https://img.shields.io/badge/platform-iOS-lightgrey.svg)
[![Contact](https://img.shields.io/badge/contact-%40kdelannoy-blue.svg)](https://twitter.com/kdelannoy)

KDEDateLabel is an UILabel subclass that saves you from refreshing it when using 'time ago' format.
![Example](example.gif)

## Installation

You have multiple choices here:
* Copy `KDEDateLabel.swift` in your project.
* Adding it in your Podfile `pod 'KDEDateLabel'`

## Usage
```swift
let label = KDEDateLabel(frame: CGRect(x: 0, y: 0, width: 100, height: 20))
label.date = NSDate()
label.dateFormatTextBlock = { date in
    return "\(Int(fabs(date.timeIntervalSinceNow)))s ago"
}
```

KDEDateLabel is also compatible with Storyboard/XIB.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

The MIT License (MIT)

Copyright (c) 2015 Kevin Delannoy

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
