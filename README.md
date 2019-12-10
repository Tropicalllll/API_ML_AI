## 「 321 」：智能合影APP-PRD

|  发布日期 | 2019/11/26  |  
| :----------: | :-----------:|  
|  产品名称 |  321  |
|  文件现状 |  进行中  |
|  文件主人 | 陈佳琳  |  
|  领头设计师 | 陈佳琳  |  
|  领头开发者 | 陈佳琳  |  
|  领头测试者 | 陈佳琳 |

## 目录
* [一、加值宣言](#一、加值宣言)
* [二、核心价值](#二、核心价值（最小可行性产品）)
* [三、背景](#三、背景)
* [四、目的](#四、目的)
* [五、目标](#五、目标)
* [六、用户](#六、用户)
* [七、用户痛点](#七、用户痛点)
* [八、用户需求](#八、用户需求)
* [九、使用者交互设计](#九、使用者交互设计)
* [十、产品结构图](#十、产品结构图)
* [十一、API运用](#十一、API运用)
* [十二、AI产品概率性](#十二、AI产品概率性)
* [十三、API使用风险评估](#十三、API使用风险评估)
* [十四、产品可行性](#十四、产品可行性)
* [十五、交互需求](#十五、交互需求)
* [十六、异常流](#十六、异常流)
* [十七、非功能性需求](#十七、非功能性需求)
* [十八、结果预期](#十八、结果预期)
* [十九、清单](#十九、清单)
---
# 1-加值宣言
没人帮忙拍合照怎么办？合照太多挑不过来怎么办？到底哪一张合照大家都ok啊？能不能让照片艺术一点？「 321 」app解决的即是上述几个问题。
- Q：没人帮忙拍合照怎么办？  
A：我们有手势识别自动拍照！
- Q：合照太多挑不过来怎么办？到底哪一张合照大家都ok啊？  
A：我们可以对合照中所有人脸的颜值和情绪指数进行分析计数，然后为你识别推荐出一张最佳合照！  
- Q：能不能让照片更与众不同一点？  
A：我们不仅能对图片进行风格化处理（卡通/素描风格），还能运用抠图让您自定义合照的背景。当然基础的图像对比度、清晰度等的处理我们也通通具备！

# 2-核心价值（最小可行性产品）
- 针对日常合照中较常见难题：提供手势识别拍照服务，人脸识别为用户筛选最佳合照，达成自定义修改合照背景的功能。

# 3-背景
智能手机普及的时代，人人都可以成为“摄影师”，而拍照也成为近年来愈发流行的社交行为趋势。无论是过年的全家福，结伴出游聚会，亦或是毕业季，拍合照这一环总是少不了。但“拍照一时爽，筛选火葬场”，合照中还有最常见的四大恨：一恨大哥没睁眼；二恨小妹太狰狞；三恨表情不同步；四恨美颜不太行。拍照后要从众多合照中挑选出一张最合适最满意的合照总是要耗费很多时间，而「 321 」app的出现则很好的解决了这些难题，就让人工智能用数据直观的告诉你！

# 4-目的
让拍合照更加得心应手，与众不同

# 5-目标
#### 前期目标
1. 用户摆出指定手势，相机识别后将自动拍摄。
2. 识别所有人脸的颜值及情绪指数，总和计数从而筛选出集体的最佳合照。
3. 对筛选出的照片进行简单的美化（对比度、清晰度、移除障碍物、风格化画面处理-卡通画风格/素描风格）。
4. 运用人像分割技术使合照与原背景分离，并产出透明背景的图片，用户可为合照重新定义背景。

#### 后期目标（暂且不做）
1. 提供社交功能，邀请好友成为app用户，实现合照即拍即分享的新社交方式。
2. 通过语音唤醒相机拍摄。

# 6-用户
交际花、毕业生、企业员工、舞台演出者、偶像团体等日常有合照需求的受众

# 7-用户痛点
- 场景1：大家都聚在一次准备拍照时，发现没有旁人能帮忙拍 
- 场景2：合照太多挑不过来，不知道到底哪张合照上所有人的表情都是过关的 
- 场景3：看着朋友圈上千篇一律的合照，追求个性的你希望自己发的合照能跟别人有所区别，更独特一点

# 8-用户需求（使用人工智能的加值是否反映到需求列表）
|  用户需求 | 可行API  |  重要程度 |
| :----------: | :-----------:|  :-----------:|
|  用户希望可以远程触发相机拍合照 |  百度-手势识别API  | 重要 |
|  用户希望可以快速又靠谱的选择出一张最佳合照 |  科大讯飞-颜值识别API  | 重要 |
|  用户希望合照更具特色和个性 | 百度-人像分割API  | 重要 |  
|  用户想简单的美化一下合照 | 百度-图像效果增强API  | 次重要 |  
#### 具体应用场景
- **场景1**：春节这天小豆把家人们集合到庭院，打算拍张新年全家福。家人们都站好了位置，这时小豆发现：可没人帮我们拍呀？突然想起前几日朋友安利给她一个合照神器 ——「 321 」app，打开首页即有手势识别拍照。以往定时拍照不是秒数太短得赶紧跑，就是秒数太长大家等到表情都僵了，现在有了手势识别拍照就可以自如的“手势一到位，想拍即拍”。
- **场景2**：假期小豆约上好友外出游玩，大家一起拍了许多合影。晚上准备发朋友圈，对着堆积成山的照片们小豆一张张翻着也不知道选哪张最好。这时又想起好友安利的「 321 」app，据说它可以批量识别同场景的合照中所有人的表情，并分析筛选出一张最佳合照。小豆跟着操作提示很快便选出了一张最满意的合照。
- **场景3**：朋友圈一刷，小豆发现姐妹们发的照片都差不多，追求独特的他希望自己发的照片能是与众不同的。点开「 321 」app中自定义合照背景的功能，为合照换上全新风格。
# 9-使用者交互设计

# 10-产品结构图
![「321」合影APP产品结构图.png](https://upload-images.jianshu.io/upload_images/9515896-90215764eee68cc9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

# 11-API运用
1. 手势唤醒相机拍照（百度-图像技术-人体分析-[手势识别](https://ai.baidu.com/docs#/Body-API/6fe80662)）
- 输入
```
import urllib.request
import urllib.parse
import base64
import json
root_url = 'https://aip.baidubce.com/rest/2.0/image-classify/v1/gesture'
img_url = 'heartsignal.jpg'

#获取access_token
def get_access():
    host = 'https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id=cqWQ1mlsHkPhI0rqxCaBhVB8&client_secret=BdgwHAaSQMQ2njK530bT7g7x3sGwfuGp'
    request = urllib.request.Request(host)
    request.add_header('Content-Type', 'application/json; charset=UTF-8')
    response = urllib.request.urlopen(request)
    content = response.read()
    content = json.loads(content)
    print('获取access_token：'+content['access_token'])
    return content['access_token']


#图片加载
def get_img(img_url):
    with open(img_url, 'rb') as f:
        if f:  
            return base64.b64encode(f.read())   
        
#获取request    
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
- 输出
```
获取access_token：24.1674ee83593888ed3c24b0f9309155b6.2592000.1578586072.282335-17993087
Out[11]:
{'log_id': 3380443945645651755,
 'result_num': 2,
 'result': [{'probability': 0.5913590788841248,
   'top': 80,
   'height': 92,
   'classname': 'Rock', #检测手势为“Rock”手势
   'width': 72,
   'left': 297},
  {'probability': 0.5343194007873535,
   'top': 39,
   'height': 74,
   'classname': 'Face', #原图该人无手势，显示为“Face”参数
   'width': 82,
   'left': 204}]}
```
2. 人脸识别最佳表情合照（科大讯飞-[颜值识别/表情识别](https://www.xfyun.cn/doc/face/face-feature-analysis/face_scoreAPI.html#接口说明)）
3. 为合照换背景（百度-图像技术-人体分析-[人像分割](https://ai.baidu.com/docs#/Body-API/top)）
4. 简易修图：图像去雾、图像对比度增强、图像风格转换、图像修复、图像清晰度增强（百度-图像技术-[图像效果增强](https://ai.baidu.com/docs#/ImageProcessing-API/top)）
5. 语音唤醒相机拍照（科大讯飞-语音识别-[语音唤醒](https://www.xfyun.cn/services/awaken?type=awaken)）

# 12-AI产品概率性
# 13-API使用风险评估
# 14-产品可行性
# 15-交互需求
# 16-异常流
# 17-非功能性需求
# 18-结果预期
# 19-清单
