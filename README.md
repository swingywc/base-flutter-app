# isaiah_flutter_app

- ### Requirement

    - [x] Xcode 9.4 or above
    - [x] Android Studio 3.0 or above (install `Flutter` and `Dart` plugins, [click here](https://flutter.io/get-started/editor/) to learn how to install plugins)

Getting Started
------

1. Follow this link ([click here](https://flutter.io/setup-macos/)) to get flutter sdk and install it.
2. Add following lines to your `.bashrc` or `.zshrc`:

    ```
      export ANDROID_SDK=$HOME/Library/Android/sdk
      export PATH=$ANDROID_SDK/emulator:$ANDROID_SDK/tools:$PATH
    ```

3. Run following commands in your terminal:

    ```
      sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer
      sudo xcodebuild -license
    ```

4. Restart your terminal to get latest resources and paths.

Run Application
------

> You can run application to iOS and Android devices using Android Studio!

### Commands

- #### Android emulator

    `emulator -list-avds`

    List all possible Android emulators that you can call and its ID.

    `emulator -avd <EMULATOR_ID> &`

    Turn on specified Android emulator by `ID`. If you have encountered crashed problem on emulator, quit emulator and use this command again with `-wipe-data` as parameter to get a clean emulator.

- #### iOS simulator

    `open -a Simulator`

    Turn on iOS simulator.

- #### Building release

    `./scripts/bump <VERSION_NAME>`

    Bump both iOS and Android to specific version name and code. If you want different version code, add `<VERSION_CODE>` at last of this command.

    `./scripts/build android`

    Build Android apk file. Add `config=development` to use development config. Default config is `production`.

Flutter
------

For help getting started with Flutter, view our online
[documentation](https://flutter.io/).
