# React Native Mobile Setup

A script to bootstrap React Native development environments targeting mobile. 

## Table of Contents

- [Requirements](#requirements)
- [Usage](#usage)
- [Support](#support)
- [Contributing](#contributing)
- [Installation](#installation)

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

## Installation 

1. Homebrew
    ```
    brew tap ccarpenter-indeed/rn-mobile-setup
    brew install ccarpenter-indeed/rn-mobile-setup/rn-mobile-setup
    ```
    > Homebrew installation adds the rn_mobile_setup script to your $PATH, meaning it can be invoked anywhere on your system.
2. NPM
    ```
    npm install @ccarpenter-indeed/rn-mobile-setup
    ```
    > NPM installation will add a dependency in the node_modules folder for whichever project your are in when you run the installation command. To invoke the script, you will need to link to the path of the script (./node_modules/@ccarpenter-indeed/rn-mobile-setup/rn_mobile_setup)
    
## Usage

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
4. Keep an eye on your terminal. Depending on your installation options the script may prompt you for required information.

## Support

Please [open an issue](https://github.com/ccarpenter-indeed/rn-mobile-setup/issues) for support.

## Contributing

Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ccarpenter-indeed/rn-mobile-setup/pulls).
