# Table of Contents

- [SignatureView](#section-id-4)
  - [Description](#section-id-10)
  - [Demonstration](#section-id-16)
  - [Requirements](#section-id-26)
- [Installation](#section-id-32)
  - [CocoaPods](#section-id-37)
  - [Carthage](#section-id-63)
  - [Manual Installation](#section-id-82)
- [Getting Started](#section-id-87)
  - [Create object of signature view](#section-id-90)
  - [Set view object as signature view](#section-id-104)
  - [Customise the signature view](#section-id-112)
  - [Capture signature view as UIImage](#section-id-132)
  - [Clear signature view](#section-id-150)
- [Contributions & License](#section-id-156)


<div id='section-id-4'/>

#SignatureView

[![Swift 3.0](https://img.shields.io/badge/Swift-3.0-orange.svg?style=flat)](https://developer.apple.com/swift/) [![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage) [![CocoaPods](https://img.shields.io/cocoapods/v/SignatureView.svg)](http://cocoadocs.org/docsets/SignatureView) [![License MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat)](https://github.com/Carthage/Carthage) [![Build Status](https://travis-ci.org/EngrAhsanAli/SignatureView.svg?branch=master)](https://travis-ci.org/EngrAhsanAli/SignatureView) 
![License MIT](https://img.shields.io/github/license/mashape/apistatus.svg) [![CocoaPods](https://img.shields.io/cocoapods/p/SignatureView.svg)]()


<div id='section-id-10'/>

##Description


SignatureView is a simple UIView to capture digital signature by drawing it on screen easily in iOS, written in Swift. It is a customised storyboard based UIView class that allows to capture digital signature easily without writing code.


<div id='section-id-16'/>

##Demonstration



![](https://github.com/EngrAhsanAli/SignatureView/blob/master/Screenshots/demo.gif)


To run the example project, clone the repo, and run `pod install` from the Example directory first.


<div id='section-id-26'/>

##Requirements

- iOS 13.0+
- Xcode 14.0+
- Swift 4+

<div id='section-id-32'/>

# Installation

`SignatureView` can be installed using Carthage, or manually.


<div id='section-id-37'/>

<div id='section-id-63'/>

##Carthage

To install Carthage, run (using Homebrew):
```
$ brew update
$ brew install carthage
```
Then add the following line to your Cartfile:

```
github "IbrahimGedami/SignatureView" "master"
```

Then import the library in all files where you use it:
```swift
import SignatureView
```


<div id='section-id-82'/>

##Manual Installation

If you prefer not to use either of the above mentioned dependency managers, you can integrate `SignatureView` into your project manually by adding the files contained in the Classes folder to your project.


<div id='section-id-87'/>

#Getting Started
----------

<div id='section-id-90'/>

##Create object of signature view

Drag `UIView` object from the *Object Library* into your `UIViewController` in storyboard.

![](https://github.com/EngrAhsanAli/SignatureView/blob/master/Screenshots/Step1.png)

<div id='section-id-104'/>

##Set view object as signature view

Set the view's class to `SignatureView` in the *Identity Inspector*.
Make sure the module property is also set to  `SignatureView`.

![](https://github.com/EngrAhsanAli/SignatureView/blob/master/Screenshots/Step2.png)

<div id='section-id-112'/>

##Customise the signature view

You can customise the rating bar appearance in the *Attributes Inspector.* 

> Note: If storyboard does not show the stars click *Refresh All Views* from the *Editor menu*.

![](https://github.com/EngrAhsanAli/SignatureView/blob/master/Screenshots/Step3.png)

<div id='section-id-132'/>

##Capture signature view as UIImage

You can capture the signature view as UIImage .

```swift
if let image = signatureView.signature {
// captured image of signature view
}
```

> You can check if signature view is empty or not using simple property `signatureView.isEmpty`.

<div id='section-id-150'/>

##Clear signature view

You can clear the signature view by calling `clear()` function.

```swift
signatureView.clear()
```

<div id='section-id-156'/>

#Contributions & License

`SignatureView` is available under the MIT license. See the [LICENSE](./LICENSE) file for more info.

Pull requests are welcome! The best contributions will consist of substitutions or configurations for classes/methods known to block the main thread during a typical app lifecycle.


