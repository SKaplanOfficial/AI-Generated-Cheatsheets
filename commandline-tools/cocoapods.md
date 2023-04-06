# CocoaPods Cheatsheet

## Overview
CocoaPods is a dependency manager for iOS and macOS projects.

## Installation
```bash
sudo gem install cocoapods
```

## Basic Usage
1. Create a new Xcode project or navigate to an existing one.
2. Create a new file called `Podfile` in the root directory of your project.
3. Add your desired dependencies to the `Podfile`.
4. Install the dependencies by running `pod install` in the terminal.

## Podfile Syntax
```ruby
# Uncomment the following line to define a global platform for your project
# platform :ios, '9.0'

target 'MyApp' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for MyApp
  pod 'Alamofire'
  pod 'SwiftyJSON', '~> 4.0'
end
```
- The `platform` keyword sets the minimum iOS or macOS version for your project.
- The `target` keyword specifies the Xcode target to install the dependencies for.
- The `use_frameworks!` keyword enables dynamic framework integration.
- The `pod` keyword specifies the name of the dependency and an optional version specifier.

## Commands
- `pod install`: Installs the dependencies specified in the `Podfile`.
- `pod update`: Updates the dependencies to their latest versions.
- `pod search`: Searches the CocoaPods repository for a specific dependency.
- `pod init`: Creates a new `Podfile` in the current directory.

## Resources
- [CocoaPods website](https://cocoapods.org/)
- [CocoaPods Guides](https://guides.cocoapods.org/)
- [CocoaPods Specs repository](https://github.com/CocoaPods/Specs)