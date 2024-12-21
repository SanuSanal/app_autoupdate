app_autoupdate helps users to donwload and install app update from GitHUb releases.

## Features

Download latest update from GitHub releases and install it. Before installing a confirmation dialog will be shown
## Getting started

Before using the package make sure there are sufficient permissions added in AndroidManifest.xml
```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.REQUEST_INSTALL_PACKAGES" />
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
```

## Usage

Call the widget inside build method
```dart
AppUpdateWidget(
    owner: '<repo-owner>',
    repo: '<repository-name>',
    onUpdateComplete: () {
        setState(() {
            // Handle update completion
        });
    }
)
```

## Additional information
Repo url :https://github.com/SanuSanal/app_autoupdate
