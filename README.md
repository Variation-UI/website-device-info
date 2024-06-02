Device Information JSON Files for Webiste.

## HOW TO USE?
Device Info Json

```javascript
const requestURL = "https://raw.githubusercontent.com/Variation-UI/website-device-info/main/json/BRAND/CODENAME.json";
```
The `requestURL` is below the **`<head>`** tag on the corresponding [**device** (Ues OPKONA as an example)](varia.org.cn/get/opkona/) page, where you should modify the link to the corresponding raw link, rather than importing it again.

CHANGELOG MarkDown

```html
const requestURL = "https://raw.githubusercontent.com/Variation-UI/website-device-info/main/json/BRAND/CODENAME.json";
```
The `requestURL` is below the **`<head>`** tag on the corresponding [**device** (Ues OPKONA as an example)](https://varia.org.cn/get/opkona/) page, where you should modify the link to the corresponding raw link, rather than importing it again.


## DEVICE INFO Json
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
    "changelog_page_link": "https://raw.githubusercontent.com/Variation-UI/website-device-info/main/markdown/BRAND/CODENAME/DATE.html"
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

## CHANGELOG MarkDown

Edit your markdown text in `<textarea>`

> [!IMPORTANT]
> incorrect indentation will result in incorrect parsing

> [!CAUTION]
> You should not add tables to markdown documents, as this will cause the document to render incorrectly
