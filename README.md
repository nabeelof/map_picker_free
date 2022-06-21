A flutter place search and location picker plugin that uses Open Street Map.
it is completely free and easy to use.

## Features

* Pick location from map
* Search location by places
* Easy to use




## Demo
![flutter_open_street_map](https://user-images.githubusercontent.com/69592754/174075388-684404cf-ada9-4c44-a1c2-5fc9fcc872ba.png)


<!-- ## Help Maintenance

I've been maintaining quite many repos these days and burning out slowly. If you could help me cheer up, buying me a cup of coffee will make my life really happy and get much energy out of it.

<a href="https://www.buymeacoffee.com/MubasharHusain" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a> -->

## Objective
This lib was designed to use open street map to set location on Flutter applications for all platforms.

## Getting Started


Import the following package in your dart file

```dart
import 'package:map_picker_free/map_picker_free.dart';
```

To use is simple, make a screen for showing it in body. And in onPicked() just return that pickedData object with Navigator.pop. You need to pass the default center position of the map and a onPicked method to get the picked position from the map.

    MapPicker(
          center: LatLong(5, 10),
          onPicked: (pickedData) {
            Navigator.pop(context, pickedData);
          })

# Then Usage

Now if you press Set Current Loatiion button, you will get the pinned location by onPicked method.

In the onPicked method you will receive pickedData.

pickedData has two properties.

1. latLong
2. address

latLong has two more properties.

1. latitude
2. longitude

For example

    MapPicker(
          center: LatLong(5, 10),
          onPicked: (pickedData) {
            Navigator.pop(context, pickedData);
          })

You can get latitude, longitude and address like that.
