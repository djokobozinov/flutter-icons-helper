# FlutterIconsHelper

In case you have the name for the icon(from [Material Icon class](https://api.flutter.dev/flutter/material/Icons-class.html)), like string. For example returned from api, like this:
```
{
  "iconName": "home"
}
```

You can display them in application in this way: 
```
Row(
  mainAxisAlignment: MainAxisAlignment.spaceAround,
  children: <Widget>[
    Icon(
      IconsHelper.iconMap['home'],
      color: Colors.pink,
      size: 24.0
    ),
    Icon(
      IconsHelper.iconMap['access_alarm_sharp'],
      color: Colors.green,
      size: 30.0
    )
  ],
)
```

If you reference all icons, all of them will be in your bundle. So pick only the icons you need to keep them in the Map.
