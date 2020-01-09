# [20x20ppt展示（171013096詹晓燕）](https://raw.githubusercontent.com/xlayal/Art_Gallery_Tour/master/20x20.pptx)

# 美术馆导览APP
 |  发布日期 | 2019-11-30 |
 | -- | -- |
 |  项目名称 | Art Gallery（美术馆导览APP） |
 |  项目现状 | 已完成 |
 |  项目的迭代 | 3_1|
 |  项目的主人 | 詹晓燕|

## 一、价值主张设计
### 1、加值宣言
#### 在信息迅速发展的背景下，人们对文化的需求程度日益加深，越来越多的人走进美术馆馆。然而大型美术馆馆存在的结构复杂、客流量大等问题。因此, 一款能够通过支持手机端的智能美术馆馆导览系统APP就可以减轻这些问题，同时为用户提供了更加方便、高效的观展体验。基于现状，通过高德的地图API、通用物体和场景识别API、人流量监控API对博物馆的导览系统进行优化。

#### 功能优先级说明
 |  优先级 | 次优先 |
 | -- | -- |
 |  基于区域人流量统计技术模型，运用百度AI中的人流量统计功能，通过照片或者视频上传对区域人流量进行统计并且在地图上显示人流量的热力图。 | 运用物体和场景识别API，对美术馆内的展品进行拍照或者照片上传，返回大类及细分类的名称结果，同时也可以获取图片识别结果对应的百科信息，返回百科词条URL、图片和摘要描要。|


### 2、核心价值
#### 本产品着眼于优化美术馆的导览推荐系统，解决用户对美术馆游览的基本需求以及协助美术馆的工作人员进行人流量统计。

### 3、项目目的
#### 一个专注于构建艺术与公众新型互动的APP

### 4、核心价值与用户痛点
 |  核心价值 | 用户痛点说明 |
 | -- | -- |
 |  **便捷性** | 参观者可以不用通过美术馆内的纸质版游览指南，只需要通过手机就可以获知美术馆的展览位置，以及及时获知当前人流分布，根据自己需求选择位置观展。 |
 |  **可视化** | 当代大型室内美术馆存在布局复杂、客流量大且不稳定的问题，智能美术馆APP可以通过客流量统计并生成热力图呈现在地图上，反馈给用户，将数据变为可视化，让用户可以直观了解到美术馆当前人流量。 |



### 5、人工智能概率性与用户痛点 
* #### 百度AI人流量识别功能的保障：
##### 1、算法领先，高精度头肩检测算法，准确率90%以上，静态人数统计不限人数，适应各种人群密集场所。
##### 2、服务稳定，可提供企业级稳定、精确的大流量服务，拥有毫秒级识别响应能力及99.9%的可靠性保障。
#### **据此，该产品人流量识别功能准确率有保障，通常不会出现与实际数据偏差太大的情况，但是由于此功能以外的因素（如网络延迟或者卡顿无法使视频图像被正确识别）会导致数据输出延迟或者不准确，此概率事件可以通过改进得到缓解，对用户的负面影响不会过大。**
* #### 百度AI中的通用物体和场景识别技术有三大产品优势：
##### 1、准确性高，基于百度海量数据，利用深度学习技术及高精度算法不断迭代模型，准确率业界领先。
##### 2、标签体系丰富，可识别出10万+物体及场景标签，并在不断丰富中，持续提供更精细的识别服务。
##### 3、简单易用，支持标准化接口封装，调用简单，只需上传单张图片，即可获取识别结果。
#### **因此，该APP用户通过拍照上传，使用了通用物体和场景识别照片中的物体返回大类及细分类的名称结果。此功能技术准确率较高，普遍情况下返回结果比较精准。但由于一些环境因素（如光线太暗）或者照片原因（如照片不清晰、识别主体精确等）造成返回识别结果不准确的状况，这些事件为小概率事件，对用户体验的负面影响不会压过正面影响的机率。**

### 6、需求列表与人工智能API加值
|  用户需求  | API接口  | 重要程度  |
|  ----  | ----  | ----  |
| 去观展之前提前预知当前馆内人流量  | 人流量监控API | 重要 |
| 寻找馆内观看人数较少的展览位置 | 地图API、 人流量监控API | 重要 |
| 馆内工作人员统计每日进馆人流量| 人流量监控API | 重要 |
| 查看馆内展品介绍| 通用物体和场景识别API | 次重要  |
##### 具体应用场景
##### 1、学生小明今天想去美术馆游览，但是不知道现在人流量如何，小明想安静地看展，这时她打开手机，点开了智能美术馆APP，查询了现在美术馆内的游客热力图，发现只有一个区域显示红色，证明游客们可能在一个展区聚集比较多，其他展区还好，接下来小明关掉手机前往美术馆。
##### 2、自由工作者小南正在艺术馆观看展览，他看到一个很独特的展品但是他不知道具体的用处，他从口袋拿出手机点开智能美术馆APP，单击“拍照识图”按钮，对着展品拍了一张照片，手机返回图片识别结果对应的展品信息。
##### 3、美术馆的工作人员老王想知道美术馆内的进馆游客数据统计，他点开智能美术馆APP的数据统计，能看到关于今日美术馆的各个展厅提供独立的参观者出入数据。
##### 4、还是老王，当区域人数超过一定数值时，系统会自动发出警报实现“浪涌人流超标告警”，帮助馆工作人员及时实行疏散策略，适当引导人流，实现错峰入馆，提升参观体验。保障潜在的参观者聚集区域，长期处于安全通畅的环境中。

## 二、产品设计原型
### 1、交互及界面设计
* #### app名称（Art Gallery）和icon设计
![icon&banner](https://upload-images.jianshu.io/upload_images/9412832-7161356c923bb3f0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* #### 人流量热力图界面设计原型（首页）和拍图识别功能
![首页&拍图识别](https://upload-images.jianshu.io/upload_images/9412832-0f25a0d1be550a04.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* #### 拍图识别物体界面设计及交互应用流程
![流程1](https://upload-images.jianshu.io/upload_images/9412832-8ff0ded05805a489.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![流程2](https://upload-images.jianshu.io/upload_images/9412832-ffcfb31bc6fb39f7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

 * #### 展览及我的功能界面
![其他功能界面](https://upload-images.jianshu.io/upload_images/9412832-3e0fa27816b18e30.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


### 2、信息设计
![api输出信息1](https://upload-images.jianshu.io/upload_images/9412832-167cc9b7db9fbccb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![api输出信息2](https://upload-images.jianshu.io/upload_images/9412832-66cd8b7bc635d8c8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 3、产品架构图
![产品架构图](https://upload-images.jianshu.io/upload_images/9412832-5680af2dd3c74a83.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 4、原型文档 
#### 1、展示页面连接：[http://xlayal.gitee.io/art_gallery](http://xlayal.gitee.io/art_gallery)

#### 2、原型文档下载：[美术馆导览APP原型文件](https://gitee.com/xlayal/art_gallery)

### 5、口头操作说明 
大家好！今天为大家介绍一款美术馆导览产品，此产品有两个使用到人工智能技术的功能——人流量识别和通用物体和场景识别。首先第一个功能，用户通过选择自己想去观展的美术馆地点，我们通过对此地方的人流量分析数据生成的热力图，通过地图可视化的界面返回给用户，简单来说，用户只要在地图上选择对应的美术馆，就可以看到此地方的人流量及分布密度。第二个功能我们简称它为“拍图识别”，在美术馆看到不认识的展品，只需点开拍照扫描的功能按钮，通过拍摄这个展品，通过返回识别出来的结果给用户。

## 三、API 产品使用及输出展示
### 1、API展示说明及输出 
##### （1）人流量统计识别（使用百度API）
* 人脸与人体识别——人流量统计API
* 接口描述：统计图像中的人体个数和流动趋势，以头肩为主要识别目标统计人数，无需正脸、全身照，适应人群密集、各种出入口场景。
摄像头硬件选型无特殊要求，分辨率建议720p以上，更低分辨率的图片也能识别，只是效果可能有差异。暂不适用夜间红外监控图片，后续会考虑扩展。（需和各艺术馆协商提供实时监控视频图像，此API示例以某艺术馆人流图为例）
* 接口地址:   [百度AI人体分析之人流量统计API](https://ai.baidu.com/ai-doc/BODY/7k3cpyy1t)
* 请求方式：POST
* 请求URL： https://aip.baidubce.com/rest/2.0/image-classify/v1/body_num
* 输入代码示例

```
Python代码示例

# encoding:utf-8

import requests
import base64

'''
人流量统计
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/body_num"
# 二进制方式打开图片文件
f = open('human.jpg', 'rb')  #上传人流量图像
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[此处输入你获取到的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
*  输出代码
```
{'person_num': 14, 'log_id': 8386600918089470214}  #识别图像中的人流量数字结果
```
##### （2）美术馆内物品识别（使用百度API）
* 图像技术——通用物体和场景识别API
* 接口描述：该请求用于通用物体及场景识别，即对于输入的一张图片（可正常解码，且长宽比适宜），输出图片中的多个物体及场景标签。
* 接口地址:   [百度API之通用物体和场景识别](https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Xk3bcxe21)
* 请求方式：POST
* 请求URL：https://aip.baidubce.com/rest/2.0/image-classify/v2/advanced_general
* 输入代码示例
```
# encoding:utf-8

import requests
import base64

'''
通用物体和场景识别
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v2/advanced_general"
# 二进制方式打开图片文件
f = open('thing.png', 'rb')  #上传想识别物体的照片
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[此处输入你的access_token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
* 输出代码示例
```
输出照片识别结果
{'log_id': 5158032026904985894, 
'result_num': 5, '
result': [{'score': 0.225492, 'root': '商品-玩具', 'keyword': '风筝'}, 
{'score': 0.171649, 'root': '商品-工艺品', 'keyword': '工艺品'}, 
{'score': 0.111659, 'root': '植物-其它', 'keyword': '盆栽植物'},
{'score': 0.057829, 'root': '非自然图像-彩色动漫', 'keyword': '卡通动漫人物'}, 
{'score': 0.004665, 'root': '动物-其他', 'keyword': '鸟类'}]}
```
### 2、使用比较分析
#### *  Face++ 中的身体检测
* 开放平台使用链接：[https://www.faceplusplus.com/body-detection/](https://www.faceplusplus.com/body-detection/)

![Face++_body-detection](https://upload-images.jianshu.io/upload_images/9412832-90a36ed3c1da0a80.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### * 腾讯AI多人脸检测
* 开放平台使用链接：[https://ai.qq.com/product/face.shtml#multiface](https://ai.qq.com/product/face.shtml#multiface)

![腾讯AI多人脸检测](https://upload-images.jianshu.io/upload_images/9412832-ab6b82fcfcd471a3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### * 百度AI人流量统计
* 开放平台使用链接：[https://ai.baidu.com/tech/body/num](https://ai.baidu.com/tech/body/num)

![百度AI](https://upload-images.jianshu.io/upload_images/9412832-d8fb28283d78ab74.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 百度与Face++还有腾讯AI的输出结果比较
##### （1）百度人流量识别api以头肩为主要识别目标统计人数，无需正脸、全身照，输出结果为人流量具体数据，输出数据结果和其他的api对比更加精准。
##### （2）Face++身体检测识别出图片的部分人流数据，但是输出结果没有具体的数量，以及部分人体未被识别到，返回数据部分偏差。
##### （3）腾讯AI多人脸检测输出结果为人脸识别列表，此功能劣势在于无法识别出无正脸的人体，应用在人流量识别的话输出数据结果偏差较大。


### 3、使用后风险报告
####  产品使用可行性
##### （1）技术方面可行性
* 该产品具有明确的核心价值和使用需求。
* 在多种实现产品功能的技术中，我们选择了精准度高、符合用户痛点的API加值。
* 该产品API存在小低率的技术风险，但是此小概率风险对用户体验的负面影响不会压过正面影响的机率。
##### （2）市场方面可行性
* 用户需求明显，且最小可行性功能满足需求。
* 用户群体广泛，如学生、职场人士皆可使用，产品的市场未来需求趋势在逐步增长。


#### 输入输出限制及API使用定价表
* 人流量通用识别
* 数据来源[https://ai.baidu.com/tech/body/num](https://ai.baidu.com/tech/body/num)

![人流量_调用限制及定价](https://upload-images.jianshu.io/upload_images/9412832-4fa8b651adb3c55c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 通用物体和场景识别
* 数据来源[https://ai.baidu.com/tech/body/num](https://ai.baidu.com/tech/body/num)
![物体识别_调用限制及定价](https://upload-images.jianshu.io/upload_images/9412832-fa766c49a8fbd80e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 价值主张写作
* **1句话版本**
#### 本产品着眼于优化美术馆的导览推荐系统，解决用户对美术馆游览的基本需求以及协助美术馆的工作人员进行人流量统计。

* **1分钟版本**
#### Art_Gallery美术馆导览app是专注于构建艺术与公众新型互动的APP。首先为目标用户提供了可视化人流量热力图的服务，用户只要在地图上选择对应的美术馆，就可以看到此美术馆的人流量及分布密度。帮助用户提前预知美术馆的人流量数据并且推荐用户出行时间，提升了用户的游览体验，同时馆内工作人员还可以通过此功能帮助博物馆分析数据，改善游客体验和及时疏通人流量；第二个功能我们简称它为“拍图识别”，在美术馆看到不认识的展品，只需点开拍照扫描的功能按钮，通过拍摄这个展品，通过返回识别出来的结果给用户。此功能帮助了用户更好地了解艺术品，对于游客体验来说是一次文明游览与智慧场馆的升级。
