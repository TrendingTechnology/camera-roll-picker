<h1 align="center">Welcome to @kebetoo/camera-roll-picker 👋</h1>
<p>
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
  <a href="https://github.com/bacarybruno/rn-camera-roll-picker#README.md">
    <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" target="_blank" />
  </a>
</p>

> A CameraRoll picker with support for changing the album name (groupName) and adding a video marker.
> Rewritten with performance in mind.
> Based on [react-native-camera-roll-picker](https://github.com/jeanpan/react-native-camera-roll-picker#readme)

### 🏠 [Homepage](https://github.com/bacarybruno/rn-camera-roll-picker)

## Getting started

* Install component through npm
```
$ npm install @kebetoo/camera-roll-picker --save
```

* Install CameraRoll from @react-native-community
```
$ npm install @react-native-community/cameraroll
```

* Require component
```
import CameraRollPicker from '@kebetoo/camera-roll-picker';
```

## Usage
```js
<CameraRollPicker callback={this.getSelectedImages} />
```

## Props
- `callback` : Callback function when images was selected. (is required!). Return a selected image array and current selected image.
- `initialNumToRender` : Specifies how many rows we want to render on our first render pass. (Default: 5)
- `groupTypes` : The group where the photos will be fetched, one of 'Album', 'All', 'Event', 'Faces', 'Library', 'PhotoStream' and 'SavedPhotos'. (Default: Album)
- `assetType` : The asset type, one of 'Photos', 'Videos' or 'All'. (Default: Photos)
- `selected` : Already be selected images array. (Default: [])
- `selectSingleItem` : Boolean to select only one single image at time. (Default: `false`)
- `maximum` : Maximum number of selected images. (Default: 15)
- `imagesPerRow` : Number of images per row. (Default: 3)
- `imageMargin` : Margin size of one image. (Default: 5)
- `containerWidth` : Width of camera roll picker container. (Default: device width)
- `selectedMarker` : Custom selected marker component. (Default: Ionicons checkmark-circle).
- `backgroundColor` : Set background color. (Default: white).
- `emptyText`: Text to display instead of a list when there are no photos found. (Default: 'No photos.')
- `emptyTextStyle` : Styles to apply to the `emptyText`. (Default: `textAlign: 'center'`)
- `loader` : Loader component node. (Default: `<ActivityIndicator />`)
### New props
- `groupName` : Specifies filter on group names, like 'Recent Photos', 'Whatsapp Images' or custom album titles. (Default: undefined)
- `videoMarker` : Custom video marker component. (Default: Ionicons videocam)
- `loaderColor`: Custom loader color, useful for theming the component. (Default: white)  ,
-  `loaderSize`: Loader size. (Default: 25)
- `checkPermissions` : A function to check android.permission.READ_EXTERNAL_STORAGE permission on Android. (Default: custom function based on PermissionsAndroid.request)

## Run tests

```sh
npm run test
```

## Author

👤 **bacarybruno**

* Github: [@bacarybruno](https://github.com/bacarybruno)

## Show your support

Give a ⭐️ if this project helped you!

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_