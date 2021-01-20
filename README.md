# Prevent Taking Screenshot or Record Video in Application - Flutter

### Import Package link given below

- [Flutter Window Manager Package](https://pub.dev/packages/flutter_windowmanager)

`flutter_windowmanager: ^0.0.2`

- Flutter Window Manager work only Android if you prevent also in iso refer below link
- [In IOS - Prevent taking Screenshot](https://medium.com/nerd-for-tech/prevent-screenshot-and-video-recording-in-flutter-93839325d66c)

### Write Code inside the Screen Widget

```
Future<void> secureScreen() async {
    await FlutterWindowManager.addFlags(FlutterWindowManager.FLAG_SECURE);
}

@override
void initState() {
    secureScreen();
    // TODO: implement initState
    super.initState();
}

```


