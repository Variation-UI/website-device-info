Device Information JSON Files for Webiste.

## HOW TO USE?
JavaScript
```javascript
const requestURL = "https://github.com/Variation-UI/website-device-info/json/device/oneplus/opkona.json";
```

## CONTENT SPECIFICATION
Please edit the content according to the format in the box.  
And the punctuation and capitalization formatting should not be changed.

```json
{
    "model": "Device Model, Device Model, Device Model",
    "codename": "codename",
    "device_photo": "$devicePhoto",
    "variation_version": "0.1",
    "variation_codename": "More",
    "android_version": "14",
    "android_codename": "UpsideDownCake",
    "build_time": "May 15, 2024",
    "status": "$status",
    "status_icon": "../source/get/$statusIcon",
    "update_time": "monthly",
    "img_link": "https://get.varia.org.cn/pd/local/$imageLink",
    "ota_link": "https://get.varia.org.cn/pd/local/$otaLink",
    "img_md5": "$md5",
    "avatar": "https://avatars.githubusercontent.com/...",
    "maintainer": "$userName",
    "github_url": "https://github.com/$username/"
}
```
`$md5` MD5 Key content;  
`$devicePhoto` A rendering of the appearence of the device for display;
`$status` The following content is optional: **`Active`** / **`Not Active`**;
`$statusIcon` The following content is optional: **`active.svg`** / **`notactive.svg`**.

[*./json/devices.json*](https://github.com/Variation-UI/website-device-info/blob/main/json/devices.json)
```json
"codename": {
        "model": "Device Model, Device Model, Device Model",
        "codename": "codename",
        "link": "https://varia.org.cn/get/codename",
        "photo": "https://api.varia.org.cn/"
    }
```
 
`$userName` **GitHub** User ID;  
`$imageLink` **FASTBOOT Mode** restore img file name on the servers;
`$otaLink` ZIP file name on the servers for updating system in **RECOVERY Mode**.


