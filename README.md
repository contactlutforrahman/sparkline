#sparkline

A Flutter package for sparkline charts.


## Installation

Install the latest version [from pub](https://pub.dartlang.org/packages/sparkline#-installing-tab-).

## Quick Start

Import the package, create a `Sparkline`, and pass it your data.

```dart
import 'package:flutter/material.dart';
import 'package:sparkline/sparkline.dart';

void main() {
  var data = [0.0, 1.0, 1.5, 2.0, 0.0, 0.0, -0.5, -1.0, -0.5, 0.0, 0.0];
  runApp(
    new MaterialApp(
      home: new Scaffold(
        body: new Center(
          child: new Container(
            width: 300.0,
            height: 100.0,
            child: new Sparkline(
              data: data,
            ),
          ),
        ),
      ),
    ),
  );
}
```


## Customization

### Sparkline

| Property     | Default          |
|--------------|:----------------:|
| lineWidth    | 2.0              |
| lineColor    | Colors.lightBlue |
| lineGradient | null             |

Example:

```dart
new Sparkline(
  data: data,
  lineWidth: 5.0,
  lineColor: Colors.purple,
);
```


```dart
new Sparkline(
  data: data,
  lineWidth: 10.0,
  lineGradient: new LinearGradient(
    begin: Alignment.topCenter,
    end: Alignment.bottomCenter,
    colors: [Colors.purple[800], Colors.purple[200]],
  ),
);
```
