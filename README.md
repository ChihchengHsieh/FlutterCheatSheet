# FlutterCheatSheet

# Import the package you need in the pubspec.yaml


Example:


```

dependencies:
  flutter:
    sdk: flutter
  provider: ^3.0.0
  intl: ^0.15.8
  http: ^0.12.0+2
  shared_preferences: ^0.5.3+1

```


# Tidy up the main file 


main.dart
```
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Shop4you',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: MyHomePage(title: 'Flutter Demo Home Page'),
    );
  }
}

class MyHomePage extends StatefulWidget {
  MyHomePage({Key key, this.title}) : super(key: key);

  final String title;

  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title),
      ),
      body: Center(),
    );
  }
}

```

# Setting up the folder structure

```
/models
/providers
/screens
/widgets

```

# Organising the Provider






