# EasyRefresher

[![CI Status](https://img.shields.io/travis/Pircate/EasyRefresher.svg?style=flat)](https://travis-ci.org/Pircate/EasyRefresher)
[![Version](https://img.shields.io/cocoapods/v/EasyRefresher.svg?style=flat)](https://cocoapods.org/pods/EasyRefresher)
[![License](https://img.shields.io/cocoapods/l/EasyRefresher.svg?style=flat)](https://cocoapods.org/pods/EasyRefresher)
[![Platform](https://img.shields.io/cocoapods/p/EasyRefresher.svg?style=flat)](https://cocoapods.org/pods/EasyRefresher)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

* iOS 9.0
* Swift 4.2

## Installation

EasyRefresher is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'EasyRefresher'
```

## Usage

```swift
tableView.refresh.header.addRefresher {
    self.reqeust {
        self.tableView.refresh.header.endRefreshing()
    }
}

tableView.refresh.footer = RefreshFooter(scrollView: tableView)
tableView.refresh.footer.refreshClosure = {
    self.reqeust {
        self.tableView.refresh.footer.endRefreshing()
    }
}
```

## Author

Pircate, gao497868860@gmail.com

## License

EasyRefresher is available under the MIT license. See the LICENSE file for more info.
