### If you don't know, please click here : [CmonBaby](https://www.cmonbaby.com)

## BaiduOCR ![Build Status](https://travis-ci.org/greenrobot/EventBus.svg?branch=master)

## About BaiduOCR Code

#### * initAccessToken
```java
// initAccessToken();
new OCRHelper.Builder(this)
        .listener(result -> {
            hasGotToken = true;
            LogUtils.e(result.getAccessToken());
        })
        .build()
.initAccessTokenWithAkSk();
```

#### * ocr to bankcard
```java
new OCRHelper.Builder(this)
                .cameraType(CameraActivity.CONTENT_TYPE_BANK_CARD)
                .requestCode(REQUEST_CODE_BANKCARD)
                .build()
                .toCamera();
```

#### * ocr from album
```java
new OCRHelper.Builder(this)
                .requestCode(REQUEST_CODE_PICK_IMAGE_FRONT)
                .build()
                .toAlbum();
```

#### * ocr to idcard
```java
new OCRHelper.Builder(this)
                .cameraType(CameraActivity.CONTENT_TYPE_ID_CARD_FRONT)
                .requestCode(REQUEST_CODE_CAMERA)
                .build()
                .toCamera();
```

Via Gradle:
```gradle
implementation 'com.baidu.ocr.ui:cmonbaby_ocr:1.0.0'
```

Via Maven:
```xml
<dependency>
    <groupId>com.baidu.ocr.ui</groupId>
    <artifactId>cmonbaby_ocr</artifactId>
    <version>1.0.0</version>
</dependency>
```

## License

Copyright (C) 2013-2020 Markus Junginger, Simon (https://www.cmonbaby.com)
BaiduOCR binaries and source code can be used according to the [Apache License, Version 2.0](LICENSE).
