# WebRTC libraries for iOS

This repository provides built WebRTC libraries which is configured for [WebRTC SFU Sora](https://sora.shiguredo.jp) iOS SDK.

## Supperted WebRTC Version

M78 (commit position 8, `0b2302e5e0418b6716fbc0b3927874fd3a842caf`)

## How to Use

### Carthage

Add the following line to Cartfile.

```ruby
# Without version
github "shiguredo/shiguredo-webrtc-ios"

# With Version
github "shiguredo/shiguredo-webrtc-ios" "78.8.0"
```

### CocoaPods

To retrieve the binary using CocoaPods, you need to add a `source` line at the top of the default `source` in your `Podfile`, like this:

```ruby
# ADD THIS LINE
# Make sure to put it on top of the default CocoaPods specs to override "WebRTC" reference!
source 'https://github.com/shiguredo/sora-ios-sdk-specs.git'
# This is the default source line which refers the default CocoaPods specs
source 'https://github.com/CocoaPods/Specs.git'
```

Then you can add the following line to `Podfile` as follows:

```ruby
# Without version
pod 'WebRTC'

# With version
pod 'WebRTC', '= 76.3.1'
```

### Manual Download

Available from [releases](https://github.com/shiguredo/sora-webrtc-ios/releases) page of this repository.

## "Development" version (iOS)

Some releases are always comes with its "development" variants, for example `76.3.1` and `76.3.1-dev`. Development variants are smaller binaries, which:

- bitcode is stripped off and not available
