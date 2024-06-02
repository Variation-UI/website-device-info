Device Information JSON Files for Webiste.

## HOW TO USE?
### Request JSON file
```javascript
const requestURL = "https://raw.githubusercontent.com/Variation-UI/website-device-info/main/json/BRAND/CODENAME.json";
```

The `requestURL` is below the **`<head>`** tag on the corresponding [**device** (Ues OPKONA as an example)](varia.org.cn/get/opkona/) page, where you should modify the link to the corresponding raw link, rather than importing it again.

## Json files specification

### DEVICE INFO Json
Please edit the content according to the format in the box.  
And the punctuation and capitalization formatting should not be changed.

The file name must be codename.

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
    "status_icon": "../sources/get/$statusIcon",
    "update_time": "Monthly",
    "img_link": "https://get.varia.org.cn/pd/local/$imageLink",
    "ota_link": "https://get.varia.org.cn/pd/local/$otaLink",
    "img_md5": "$md5",
    "img_size": "1.34GB",
    "avatar": "https://avatars.githubusercontent.com/...",
    "maintainer": "$userName",
    "github_url": "https://github.com/$username/",
    "changelog_last": "Merged January 2024 security patches.<br>Fix Side slider and Fix FingerPrint.",
    "changelog_history": {
        "$date": "Merged January 2024 security patches.<br>Fix Side slider and Fix FingerPrint."
    }
}
```
`$md5` MD5 Key content;  
`$devicePhoto` A rendering of the appearence of the device for display;
`$status` The following content is optional: **`Active`** / **`Not Active`**;
`$statusIcon` The following content is optional: **`active.svg`** / **`notactive.svg`**.
`$date` Release Date, Format is `Abbreviated month name + Abbreviated year first letter of English`, like: **`May,2024 -> MayTwentyFour -> MayTF`**.

The latest update log entry must be **`Last`**, and the rest should be the `$date`, although history update logs are not show on the website, but you should still keep them.

> [!IMPORTANT]
> Must add <br> when wrapping a line.

[*./device/devices.json*](https://github.com/Variation-UI/website-device-info/blob/main/device/devices.json)
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