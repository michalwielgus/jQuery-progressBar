# progressBar - jQuery Plugin

Simple jQuery plugin to create reading progress bar on given element.
### Basic usage

```html
<script src="http://code.jquery.com/jquery-3.3.1.min.js"></script>
<script src="jQuery.progressBar.min.js"></script>
```
```javascript


$('article-element').progressBar();
```

This code should create default progress bar fixed to the top of the screen and style it with default options.

### Configuration

You can customize progress by setting particular options in parameter object. Here you have default configuration:

```javascript
$('article-element').progressBar({
    throttleTime: 100,
    debounceTime: 200,
    progressBarHeight: 10,
    progressBarColor: '#F1F1F1',
    progressBarValueColor: '#A1A1A1',
    progressBarTopPosition: 0
  });
```

### Options

|  Attribute  |  Type  |  Default  |  Description  |
| ------------ | ------------ | ------------ | ------------ |
|  `throttleTime` |  Number  |  100  | Defines how often should be calculate of progress bar width (in ms). |
| `debounceTime`  |  Number |  200 | Defines the time from the last scroll event to the recalculation time of progress bar width. |
| `progressBarHeight`  |  Number  | 10  | Defines height of progress bar.  |
|  `progressBarColor`  | String  | #F1F1F1  |  Defines color of the "unread" part of progress bar (in hex notation).  |
|  `progressBarValueColor`  | String  | #A1A1A1  |  Defines color of the "read" part of progress bar (in hex notation).  |
|  `progressBarTopPosition` |  Number | 0  | Defines position of the progress bar from the top of the window(in pixels). |

