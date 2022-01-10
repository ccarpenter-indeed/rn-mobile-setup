# React Native Mobile Setup

A script to bootstrap React Native development environments targeting mobile. 

## Table of Contents

- [Requirements](#requirements)
- [Usage](#usage)
- [Support](#support)
- [Contributing](#contributing)

## Requirements
- Your project structure*
    - react-native-project
        - ios
            - ...
            - Podfile
            - .xcode-version
        - android
            - ...
            - build.gradle  

        - (script is from run here)  
    > \* While not technically required, this project structure will ensure no excess dependencies are downloaded.
- iOS development requirements
    - ~15 GB free space for XCode and simulators
    - macOS
    - A registered [Apple Developer Account](https://developer.apple.com/register/)
    - An [.xcode-version](https://github.com/xcpretty/xcode-install/blob/master/XCODE_VERSION.md) file in your ios directory detailing the targeted XCode version
    - An iOS target definition in your Podfile in the format 
        ```
        platform: ios, 'xx.yy.zz'
        ```
- Android development requirements
    - ~5 GB free space for Android Studio and simulators
    - Windows, Linux, or macOS

## Usage

This brew package will add the mobile setup script to your path, meaning it can be invoked anywhere on your system.  

To setup your project for React Native mobile development, follow these steps...

1. Navigate to the root directory of your project.
2. If you have not already done so, run
    ```
    brew tap ccarpenter-indeed/rn-mobile-setup
    brew install ccarpenter-indeed/rn-mobile-setup/rn-mobile-setup
    ```
3. Run the script using
    ```
    source rn_mobile_setup
    ```
    To see a list of optional flags, use
    ```
    source rn_mobile_setup -help
    ```
4. Keep and eye on your terminal. The depending on your installation options the script may prompt you for required information.

## Support

Please [open an issue](https://github.com/ccarpenter-indeed/rn-mobile-setup/issues) for support.

## Contributing

Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ccarpenter-indeed/rn-mobile-setup/pulls).