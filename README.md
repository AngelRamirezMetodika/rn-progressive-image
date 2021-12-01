<h1 align="center">react-native-lazy-image</h1>

<div align="center">
    <strong>An easy to use, stylistically customizable lazy-loader for react-native's image component.</strong>
</div>

<br>

<div align="center">

  <a href="https://npmjs.org/package/react-native-lazy-image">
    <img src="https://img.shields.io/npm/v/react-native-lazy-image.svg?style=flat-square" alt="npm package version" />
  </a>

  <a href="https://npmjs.org/package/react-native-lazy-image">
    <img src="https://img.shields.io/npm/dm/react-native-lazy-image.svg?style=flat-square" alt="npm downloads" />
  </a>

  <a href="https://github.com/feross/standard">
    <img src="https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square" alt="standard JS linter" />
  </a>

  <a href="https://github.com/QuintonC/react-native-lazy-image/blob/master/LICENSE.md">
    <img src="https://img.shields.io/npm/l/react-native-lazy-image.svg?style=flat-square" alt="project license" />
  </a>

  <a href="http://makeapullrequest.com">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="make a pull request" />
  </a>

  <img src="https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square" alt="All Contributors" />
</div>

<br>

<div align="center">

  <a href="https://github.com/QuintonC/react-native-lazy-image/watchers">
    <img src="https://img.shields.io/github/watchers/QuintonC/react-native-lazy-image.svg?style=social" alt="Github Watch Badge" />
  </a>

  <a href="https://github.com/QuintonC/react-native-lazy-image/stargazers">
    <img src="https://img.shields.io/github/stars/BugiDev/react-native-lazy-image.svg?style=social" alt="Github Star Badge" />
  </a>

  <a href="https://twitter.com/intent/tweet?text=Check%20out%20react-native-lazy-image!%20https://github.com/BugiDev/react-native-lazy-image%20%F0%9F%91%8D">
    <img src="https://img.shields.io/twitter/url/https/github.com/BugiDev/react-native-lazy-image.svg?style=social" alt="Tweet" />
  </a>

</div>

<br>

<div align="center">
  Built with ❤︎ by <a href="https://github.com/QuintonC">Quinton Chester</a> and <a href="https://github.com/QuintonC/react-native-lazy-image/graphs/contributors">contributors</a>
</div>

<h2>Table of Contents</h2>
  <li><a href="#install">Install</a></li>
  <li><a href="#usage">Usage</a></li>
  <li><a href="#props">Props</a></li>
  <li><a href="#contributing">Contributing</a></li>
  <li><a href="#license">License</a></li>


## Installation

```bash
$ npm install react-native-lazy-image
```

## Usage
At the top of your file:
```javascript
import LazyImage from 'react-native-lazy-image'
```

At the core, this is the simplest form of usage:
```
    <LazyImage 
        small_source={{ uri: your_image_path_here }}
        large_source={{ uri: your_image_path_here }}
    />
```

## Props
| Parameter             | Default  | Required | Description                                                                         |
| :-------------------- | :------- | :------- | :---------------------------------------------------------------------------------- |
| `small_source`        |          | true     | The source for the smallest image that will initially be blurred and animated out   |
| `large_source`        |          | true     | The source for the larger image that we will be lazily loading                      |
| `type`                | `timing` | false    | The type of animation to use. Either `spring` or `timing`.                          |
| `style`               |          | false    | The style of the image container. Images use `StyleSheet.absoluteFillObject`, so define your overall image structure here |
| `timing_config`       |          | false    | The config for the Animated.timing animation                                        |
| `spring_config`       |          | false    | The config for the Animated.spring animation                                        |
| `initial_blur_radius` | `3`      | false    | The initial blur amount for the small image. Only present until the large image has been loaded and animates in. |
| `use_native_drive`    | `true`   | false    | Specify whether you would like to use the native driver for animations. Recommended to leave this untouched as `true` is the default value. |

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please follow the issue format.

To contribute properly please use gitflow and semver standards.
1. Fork it.
2. Create your feature branch: `git checkout -b feature/feature-name`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin feature/feature-name`
5. Test code thoroughly.
6. ????
7. Submit a pull request

Or open up [an issue](https://github.com/QuintonC/react-native-lazy-image/issues).

## License
Licensed under the [MIT](https://choosealicense.com/licenses/mit/) license.