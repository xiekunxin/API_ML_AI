### 拼桌交友——人脸识别技术应用 | 2018/11/25
 ***
 负责人 | 谢坤鑫
---|---
 设计师 | 谢坤鑫
 开发者 | 谢坤鑫
 测试者 | 谢坤鑫
 ***
 ### Goals: 通过人脸识别技术为餐厅客户提供定制服务，并将数据信息整合分析，为餐厅改善服务和菜色提供数据依据
***
### Background and strategic fit（背景和战略契合度）
* 背景  
传统媒体时代，以餐饮行业为例，大多餐厅均以产品为导向，餐厅的经营重心围绕在菜肴的色香味形、器皿的造型、标准化的服务等方面。然而随着时代的发展，新生代00后的成长，餐厅能够有更多的可能，事实上，餐厅所提供的功能并不仅局限于餐饮领域，作为聚集人气最旺的场所，餐厅的社交元素很强，但其社交元素往往只是作为一种被动且潜在的延伸，甚少有餐厅主动为消费者提供社交的机会。
* 战略契合度
针对此情况，将通过机器学习技术中“人脸搜索功能”以人脸相似度作为连接点帮助用户拼桌交友，强化餐厅的“社交”属性并以此建立餐厅独特的定位价值，吸引新生代消费者。
***
### 加值宣言
* 核心：运用了机器学习中的人脸搜索功能，借助“人脸相似度”为客户提供友好的社交方式，满足客户的消费诉求并达到提高餐厅点餐效率，节省餐厅座位资源的目的
以建立社交符号，增加消费者与餐厅的互动，并建立餐厅独特的定位价值
* 特点：还将特别将以大数据思维挖掘人脸识别所收集到的用户信息的潜在价值，记录顾客男女比例以及年龄阶段和他们分别到店次数，消费时间，分析多次到店及二次消费顾客的购买频率、消费能力等相关信息，对比顾客数据的变化趋势，为经营决策提供数据参考

***
### 核心价值与用户痛点
* 最小可用产品：产品选用“拼桌交友”功能为最小可用产品，理由如下，首先，通过用户调查测试发现产品具有广泛的发展前景并被市场所接受，其次，通过实际API接口调用证实产品设想可实现并且成本最低（免费）
* 用户痛点：餐厅独自进餐感到孤单；餐厅服务千篇一律，缺乏吸引力；餐厅饮食缺乏足够的消费刺激；

### 需求列表
 用户案例 | 对应标题 | AI应用
---|--- |--- |
社交需求 | 拼桌交友| 人脸搜索 | 
***
### 使用者交互及设计: 
#### 操作流程
[![操作流程.png](https://i.loli.net/2018/12/09/5c0c811c0bf53.png)](https://i.loli.net/2018/12/09/5c0c811c0bf53.png)
#### 产品使用流程图
![产品使用流程图.png](https://i.loli.net/2019/01/05/5c30c6c0a5314.png)  
##### 异常流程 Exception Flows
* 无法登陆用户页面/用户页面登陆延时
* 拼桌交友匹配弹回错误
* 付款失败/付款延时
解决方案 Solution：参考链接
#### 产品功能框架图
![产品功能框架图.png](https://i.loli.net/2019/01/05/5c30cf4e87668.png)
#### axure原型
![Axure原型1.png](https://i.loli.net/2019/01/06/5c316a7f2fa16.png)
![拼桌交友.png](https://i.loli.net/2019/01/06/5c316b28ad269.png)
***
### API展示
* 关于API测试（web demo）
![例子1.png](https://i.loli.net/2019/01/06/5c316c7760154.png)  
##### 说明：使用7组数据做对比，其中男女比例为5:2，于数据库输入俯拍，仰拍，正脸照，以及搞怪的表情做数据模型对比分析，测试产品功能人脸识别准确率受不同因素干扰程度    
干扰因素| 光线 | 俯拍 | 仰拍 | 微表情 | 表情扭曲 | 
---|--- |--- |
影响程度 | 较小| 较小 | 较小 | 较小 | 较大
详细资料参见

 --- 
* 关于API调用（[代码链接](https://github.com/xiekunxin/API_ML_AI/blob/master/image/2019-01-05_182318.png)）
##### 服务平台：百度AI
##### AI产品：人脸搜索  
![2019-01-05_182404.png](https://i.loli.net/2019/01/05/5c309e75c2638.png)
 --- 
*** 
### API产品使用对比
在目前API人脸识别产品市场中，根据产品开发成熟程度并各综合各人工智能类人脸识别产品的下载量、知名度、竞争力等情况考虑，选出竞品为“百度AI”和“face+++”。将“颜鉴”以及“宇泛智能”列为次级竞品作适当分析   
* 竞品对比明细：![微信图片_20181220200001.png](https://i.loli.net/2018/12/20/5c1b8468f2c66.png)  
#### 准确率辨析：
国际人脸识别评估集LFW榜， face++ 99.5% , 商汤 99.53% ， 腾讯 99.65% , 百度 99.77%，中科奥森 99.77% , 中科云从 99.5%， 颜鉴99.64%，北京飞搜科技 99.4% ,宇泛智能 99%
* 准确率：百度AI为众多产品中准确率最高的一款产品，相对Face+++在准确率上更胜一筹，然而值得一提的是，Face+++自身的准确率也达到了较高的水平，能够基本满足餐厅人脸识别的技术要求
