## 「 321 」：智能合影APP-PRD

|  发布日期 | 2019/11/26  |  
| :----------: | :-----------:|  
|  产品名称 |  321  |
|  文件现状 |  进行中  |
|  文件主人 | 陈佳琳  |  
|  领头设计师 | 陈佳琳  |  
|  领头开发者 | 陈佳琳  |  
|  领头测试者 | 陈佳琳 |

# 第一部分 价值主张
### 1. 加值宣言
#### 一句话版本
解放双手拍照，从这一刻开始

#### 一段话版本
没人帮忙拍合照怎么办？合照太多挑不过来怎么办？到底哪一张合照大家都ok啊？能不能让照片艺术一点？「 321 」app解决的即是上述几个问题。
- Q：没人帮忙拍合照怎么办？  
A：我们有手势识别自动拍照！
- Q：合照太多挑不过来怎么办？到底哪一张合照大家都ok啊？  
A：我们可以对合照中所有人脸的颜值进行分析统计，为你识别推荐出一张最佳合照！  
- Q：能不能让照片更与众不同一点？  
A：我们不仅能对图片进行风格化处理（卡通/素描风格），还能运用抠图让您自定义合照的背景。当然基础的图像对比度、清晰度等的处理我们也通通具备！

### 2. 核心价值（最小可行性产品）
- 针对日常合照中较常见难题：提供手势识别拍照服务，人脸识别为用户筛选最佳合照，达成自定义修改合照背景的功能。

# 第二部分 市场分析
### 一、市场背景
在颜值时代，拍照和晒照已经是用户日常娱乐生活的一部分，移动社交媒体也在催生用户的拍照需求。智能手机普及的时代，人人都可以成为“摄影师”，而拍照也成为近年来愈发流行的社交行为趋势。无论是过年的全家福，结伴出游聚会，亦或是毕业季，拍合照这一环总是少不了。但“拍照一时爽，筛选火葬场”，合照中还有最常见的四大恨：一恨大哥没睁眼；二恨小妹太狰狞；三恨表情不同步；四恨美颜不太行。拍照后要从众多合照中挑选出一张最合适最满意的合照总是要耗费很多时间，而「 321 」app的出现则很好的解决了这些难题，就让人工智能用数据直观的告诉你！

# 第三部分 产品说明
## 1. 定位

## 2. 问题（用户痛点）
- 场景1：大家都聚在一次准备拍照时，发现没有旁人能帮忙拍 
- 场景2：合照太多挑不过来，不知道到底哪张合照上所有人的表情都是可以的 
- 场景3：看着朋友圈上千篇一律的合照，追求个性的你希望自己发的合照能跟别人有所区别，更独特一点

## 3. 目标
1. 让用户不用触摸移动设备屏幕也能拍照
2. 减少用户筛选照片的时间，提高选中率
3.  实现更加独一无二的照片效果

## 4. 目标用户
交际花、旅行团、企业员工（年会/团建）、舞台演出者等所有有合照需求的人群
- 用户特征：喜欢社交、拍照；追求个性、审美；热衷分享生活；对照片质量有一定要求；关照朋友（图片上是否好看）；能较熟练使用移动设备及APP功能

## 5. 用户需求
**（使用的人工智能要反映到需求列表中）**
|  用户需求 | 可行API  |  重要程度 |
| :----------: | :-----------:|  :-----------:|
|  用户希望可以远程触发相机拍合照 |  百度 - 手势识别API  | 重要 |
|  用户希望可以快速又靠谱的选择出一张最佳合照 |  Face++ - 颜值评分API  | 重要 |
|  用户希望合照更具特色和个性 | 百度 - 人像分割API  | 重要 |  
|  用户想简单的美化一下合照 | 百度 - 图像效果增强API  | 次重要 |  
## 6. 具体使用场景
- **场景1**：春节这天小豆把家人们集合到庭院，打算拍张新年全家福。家人们都站好了位置，这时小豆发现：可没人帮我们拍呀？突然想起前几日朋友安利给她一个合照神器 ——「 321 」app，打开首页即有手势识别拍照。以往定时拍照不是秒数太短得赶紧跑，就是秒数太长大家等到表情都僵了，现在有了手势识别拍照就可以自如的“手势一到位，想拍即拍”。
- **场景2**：假期小豆约上好友外出游玩，大家一起拍了许多合影。晚上准备发朋友圈，对着堆积成山的照片们小豆一张张翻着也不知道选哪张最好。这时又想起好友安利的「 321 」app，据说它可以批量识别同场景的合照中所有人的表情，并分析筛选出一张最佳合照。小豆跟着操作提示很快便选出了一张最满意的合照。
- **场景3**：朋友圈一刷，小豆发现姐妹们发的照片都差不多，追求独特的他希望自己发的照片能是与众不同的。点开「 321 」app中自定义合照背景的功能，为合照换上全新风格。
## 7. 功能
### 7.1 前期目标
|  功能名称 | 实现形式  |  功能优先级  |
| :----------: | :-----------|  :-----------:|
|  **拍**（为你拍照） |  用户摆出预先设置的手势，相机进行手势识别后将自动拍摄照片。  |  优先  | 
|  **挑**（帮你挑选） |  识别同一批照片或者用户自行选定的照片中所有人脸的颜值并进行评分，总和统计从而筛选出集体的最佳合照。   |  优先  |
|  **独**（让你独特）  |  运用人像分割技术使合照与原背景分离，并产出透明背景的图片，用户可为合照重新定义背景。  |  优先  |
|  **美**（给你美化）  |  对筛选出的照片进行简单的美化（对比度、清晰度、移除障碍物、风格化画面处理-卡通画风格/素描风格）。  |  次优先  |

### 7.2 后期目标（不做）
|  功能名称 | 实现形式  |  功能优先级  |
| :----------: | :-----------|  :-----------:|
|  **友**（以照会友） |  提供社交功能，邀请好友成为app用户，实现合照**即拍即分享**的**新社交方式**。  |  次优先  | 
|  **拍**（为你拍照2.0） |  实现通过语音唤醒相机拍摄。   |  次优先  |

## 8. 使用者交互设计

## 9. 产品结构图
![](https://upload-images.jianshu.io/upload_images/9515896-90215764eee68cc9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 10. API运用
### 10.1 功能一：手势唤醒相机拍照 / API运用：百度 - 手势识别
|  接口地址 |  https://ai.baidu.com/tech/body/gesture  | 
| :----------: | :-----------|  
|  接口描述 |  识别图片中的手势类型，返回手势名称、手势矩形框、概率分数，可识别24种常见手势，适用于手势特效、智能家居手势交互等场景。  |  
|  请求方法 |  POST  |
|  请求URL |  https://aip.baidubce.com/rest/2.0/image-classify/v1/gesture  |
- 输入：
```
import urllib.request
import urllib.parse
import base64
import json
root_url = 'https://aip.baidubce.com/rest/2.0/image-classify/v1/gesture' （输入请求URL）
img_url = r'C:\Users\Administrator\Documents\API\five.jpg' （输入照片路径）

# 获取access_token
def get_access():
    host = 'https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id= "输入你的API Key" &client_secret="输入你的Secret Key" '
    request = urllib.request.Request(host)
    request.add_header('Content-Type', 'application/json; charset=UTF-8')
    response = urllib.request.urlopen(request)
    content = response.read()
    content = json.loads(content)
    print('获取access_token：'+content['access_token'])
    return content['access_token']

# 图片加载
def get_img(img_url):
    with open(img_url, 'rb') as f:
        if f:  
            return base64.b64encode(f.read())   
        
# 获取request    
def get_request(url, access):
    params = {"image": get_img(img_url),"image_type": "BASE64"}
    params = urllib.parse.urlencode(params).encode('utf-8')
    request_url = url + "?access_token=" + access
    request = urllib.request.Request(url=request_url, data=params)
    request.add_header('Content-Type', 'application/x-www-form-urlencoded')
    return request

if __name__ == '__main__':
    response = urllib.request.urlopen(get_request(root_url, get_access()))
    content = response.read().decode('utf-8')
    result = json.loads(content)
    
result
```
- 输出：
```
{'log_id': 1748470085008740440,
 'result_num': 4,
 'result': [{'probability': 0.9992140531539917,
   'top': 168,
   'height': 307,
   'classname': 'Five', （检测出手势为“Five”）
   'width': 225,
   'left': 158},
  {'probability': 0.9572620391845703,
   'top': 96,
   'height': 207,
   'classname': 'Face', （检测出一个人脸）
   'width': 185,
   'left': 346},
  {'probability': 0.8524100184440613,
   'top': 337,
   'height': 238,
   'classname': 'Five', （检测出手势为“Five”）
   'width': 196,
   'left': 576},
  {'probability': 0.5487503409385681,
   'top': 217,
   'height': 210,
   'classname': 'Face', （检测出又一个人脸）
   'width': 157,
   'left': 513}]}
```
- 检测结果截图：
![百度检测结果](https://upload-images.jianshu.io/upload_images/9515896-b3fa962584b9a482.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

####  ！ 竞品：Face++ - 手势识别 ！
|  接口地址  |  https://www.faceplusplus.com.cn/gesture-recognition/  |
| :----------: | :-----------| 
|  接口描述 |  调用者提供图片文件或者图片URL，检测图片中出现的所有的手部，并返回其在图片中的矩形框位置与相应的手势含义。目前可以识别 19 种手势。  |   
|  请求方法 |  POST  |
|  请求URL |  https://api-cn.faceplusplus.com/humanbodypp/v1/gesture  |
- 输入：
```
import requests
from json import JSONDecoder

http_url ="https://api-cn.faceplusplus.com/humanbodypp/v1/gesture"
key ="输入你的API Key"
secret ="输入你的API Secret"
filepath ="图片URL"

data = {"api_key": key, "api_secret": secret, "return_attributes":"gesture"}
files = {"image_file": open(filepath, "rb")}

response = requests.post(http_url, data=data, files=files)

import json
response.json()
```
- 输出：
```
{'request_id': '1577175154,ee808183-bd7c-4c2e-901d-117f6036015c',
 'time_used': 126,
 'hands': [{'hand_rectangle': {'top': 181,
    'left': 510,
    'width': 168,
    'height': 359},
   'gesture': {'beg': 0.908,
    'big_v': 0.12,
    'double_finger_up': 1.42,
    'fist': 14.36,
    'hand_open': 0.12,
    'heart_a': 0.12,
    'heart_b': 0.12,
    'heart_c': 0.12,
    'heart_d': 0.12,
    'index_finger_up': 3.07,
    'namaste': 0.595,
    'ok': 0.12,
    'palm_up': 0.12,
    'phonecall': 7.202,
    'rock': 0.75,
    'thanks': 0.396,
    'thumb_down': 0.152,
    'thumb_up': 0.192,
    'unknown': 0.452,
    'victory': 69.543}},
  {'hand_rectangle': {'top': 188, 'left': 151, 'width': 206, 'height': 296},
 
  # “gesture”：手势识别结果列表。每个字段的值是一个浮点数，范围 [0,100]，小数点后3位有效数字，总和等于100。
    'gesture': {'beg': 0,            
    'big_v': 0,
    'double_finger_up': 0.221,
    'fist': 0,
    'hand_open': 99.763,
    'heart_a': 0,
    'heart_b': 0,
    'heart_c': 0,
    'heart_d': 0.001,
    'index_finger_up': 0,
    'namaste': 0.004,
    'ok': 0.001,
    'palm_up': 0.001,
    'phonecall': 0.001,
    'rock': 0.007,
    'thanks': 0,
    'thumb_down': 0,
    'thumb_up': 0,
    'unknown': 0,
    'victory': 0}}],
 'image_id': 'Wv1j5gOy8IKdNZANfZ1aug=='}
```
- 检测结果截图：
![Face++检测结果](https://upload-images.jianshu.io/upload_images/9515896-9cd0f7754d0432de.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### ！ 手势识别API两家对比 ！
|  #  |  百度  |  Face++  |
| :----------: | :-----------|  :-----------|
|  手势数量 |  24种  |  19种  |
|  支持拍摄场景  |  **自拍、他拍**：主要适用于3米以内的自拍、他人拍摄，1米内识别效果最佳。拍摄距离太远时，手部目标太小，无法准确定位和识别。  |  **自拍**：主要适用于移动设备的自拍场景设计，在其他场景下对手势的识别精度可能不足。  |
|  自有特点  |  除识别手势外，若图像中检测到人脸，会同时返回人脸框位置。  |  对于单手的手势，不区分左右手，即无论左右手摆出此手势都会被识别。  |
|  代码运行结果  |  直接检测出图片人数以及每个人对应手势的名称。  |  返回结果为一个包括19种手势的列表，19种手势合计100分，评分最高的即为识别出的手势。  |
|  运行正确性  |  ![](https://upload-images.jianshu.io/upload_images/9515896-b3fa962584b9a482.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)同一张照片，百度能正确识别出两个手势。  |  ![](https://upload-images.jianshu.io/upload_images/9515896-9cd0f7754d0432de.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)同一张照片，Face++只识别出了男生的手势，女生的手势只识别到一半导致结果错误。  |
|  使用评价  |  结果直接显示人数及手势，直观便捷，一目了然。  |  需要在返回的结果列表中自行对比评分、寻找最高分的手势，不太直观，偶尔还会找错导致得出错误的手势结论。  |  
|  产品价格  |  ![](https://upload-images.jianshu.io/upload_images/9515896-4e46c7a681236141.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  |  ![](https://upload-images.jianshu.io/upload_images/9515896-3a1c43119b37cd31.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  |  
|  性价比  |  ★★★★★  |  ★★★  |

### 10.2 功能二：颜值识别分析最佳合照 / API运用：Face++ - 颜值评分
|  接口地址 |  https://www.faceplusplus.com.cn/beauty/  | 
| :----------: | :-----------|  
|  接口描述 |  计算检测到的人脸的颜值分数，分别返回男性和女性视角下该人脸的颜值分数。  |  
|  请求方法 |  POST  |
|  请求URL |  https://api-cn.faceplusplus.com/facepp/v3/detect  |
- 输入：
```
import requests
from json import JSONDecoder

http_url ="https://api-cn.faceplusplus.com/facepp/v3/detect"
key ="输入API Key"
secret ="输入API Secret"
filepath ="图片路径"

data = {"api_key": key, "api_secret": secret, "return_attributes":"beauty"}
files = {"image_file": open(filepath, "rb")}
response = requests.post(http_url, data=data, files=files)

import json
response.json()
```
- 输出：
```
[ 'faces': 
[{'attributes': {'beauty': {'female_score': 53.055, 'male_score': 54.965}},
 ......
 {'attributes': {'beauty': {'female_score': 49.386, 'male_score': 53.612}},
 ......
 'face_num': 2}
```
- 检测结果截图：
![](https://upload-images.jianshu.io/upload_images/9515896-98e371d512396160.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/9515896-c04be6bda75bae89.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 10.3 功能三：自定义替换照片背景 / API运用：百度 - 人像分割
|  接口地址 |  https://ai.baidu.com/tech/body/seg/  | 
| :----------: | :-----------|  
|  接口描述 |  对于输入的一张图片（可正常解码，且长宽比适宜），识别人体的轮廓范围，与背景进行分离，适用于拍照背景替换、照片合成、身体特效等场景。输入正常人像图片，返回分割后的二值结果图、灰度图、透明背景的人像图（png格式）。  |  
|  请求方法 |  POST  |
|  请求URL |  https://aip.baidubce.com/rest/2.0/image-classify/v1/body_seg  |
- 输入：
```
import requests
import base64
request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/body_seg"
# 二进制方式打开图片文件
f = open(r'C:\Users\Administrator\Documents\API\apifinal\beauty.jpg', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '输入token'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
- 输出：返回值为分割后图片的json档，返回的二值图像需要进行二次处理才可查看分割效果。
![](https://upload-images.jianshu.io/upload_images/9515896-b98cf8ed6ff4843d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 检测结果截图：
![](https://upload-images.jianshu.io/upload_images/9515896-26c4aaee3411e94e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 10.4 功能四：简易修图 / API运用：百度 - 图像效果增强
|  接口地址  |  [https://ai.baidu.com/ai-doc/IMAGEPROCESS/nk3bcloer](https://ai.baidu.com/ai-doc/IMAGEPROCESS/nk3bcloer)  |
| :----------: | :-----------| 
|  接口描述 |  图像效果增强包括：图像去雾、图像对比度增强、图像风格转换、图像修复、图像清晰度增强.  |   
|  请求方法 |  POST  |
|  请求URL |  不同功能对应不同URL  |
