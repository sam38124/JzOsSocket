[![Platform](https://img.shields.io/badge/平台-%20IOS%20-brightgreen.svg)](https://github.com/sam38124)
[![characteristic](https://img.shields.io/badge/特點-%20輕量級%20%7C%20簡單易用%20%20%7C%20穩定%20-brightgreen.svg)](https://github.com/sam38124)
# JzOsSocket
基於Java-DataStream的Socket溝通框架
## 目錄
* [如何導入到專案](#Import)
* [快速使用](#Use)

<a name="Import"></a>
## 如何導入到項目
> 支持framework導入。 <br/>

#### 1.首先將framework拉入要導入的Project當中
<img src="https://github.com/sam38124/JzOsFrameWork/blob/master/i2.png" width = "800"  alt="i1" /><a name="Use"></a>
#### 2.將三個選項打勾
<img src="https://github.com/sam38124/JzOsFrameWork/blob/master/i1.png" width = "800"  alt="i1" /><a name="Use"></a>
#### 3.選擇Embed and signed
<img src="https://github.com/sam38124/JzOsFrameWork/blob/master/i3.png" width = "800"  alt="i1" /><a name="Use"></a>
<a name="Use"></a>
## 快速使用
```swift
//必須包一個do catch來預防網路連線而引發的例外
  do{
  //建立你的stream流
            let stream=DataStream()
            //設定ip和port和還有連線timeout時間
            try stream.setStream(self.ip,self.port,10)
            //傳送utf字元
            try stream.writeUTF("hello world")
            //傳送int
            try stream.writeINT(117)
            //讀取int
            try stream.readInt()
            //讀取utf-8
            try stream.readUTf()
        }catch{
            print("連線發生異常")
        }
```

<a name="About"></a>
### 關於我
橙的電子android and ios developer

*line:sam38124

*gmail:sam38124@gmail.com
