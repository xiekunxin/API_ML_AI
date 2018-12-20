### 餐厅人脸识别应用 | 2018/11/25
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
1.中国消费水平升级以及外卖平台的崛起，逼向餐饮服务业进一提升顾客的用餐体验
2.人脸识别技术日渐成熟，该技术在餐饮服务业的应用已有许多成功案例
* 战略契合度
针对此情况，将以结合机器学习中人脸对比功能、人脸搜索功能、人脸检测与属性分析三大功能以自助点餐的形式来提升用户个性化定制化的消费诉求

***
### 用户需求
* 用户：价值观开放多元，消费理念不再局限于朴素务实，更加强调用户体验和价值认同的消费理念的新生代群体（90后，00后）
* 需求 : 未来中国餐饮业将聚焦在新生代这块，随着人们大健康意识不断提升，大健康主流消费群体以新生代为主，轻食、科技化、个性化菜单创新都是应对新生代诉求的举措。
***
### 加值宣言
* 核心：运用了机器学习中的人脸对比功能，提取用户的面部特征，与餐厅的数据库里的图片做相似度比较，判断用户身份，并依据资料提供其历史信息，VIP用户则会另外提醒至服务工作人员为其提供定制服务
* 其他：运用了机器学习中的人脸搜索功能，借助“人脸相似度”为客户提供友好的社交方式，并达到节省餐厅座位资源的目的；运用了机器学习中的人脸检测与属性分析功能，与用户进行简单而友好的互动，并以“个性化套餐”满足新生代消费者个性化定制化的消费诉求
* 特点：还将特别将以大数据思维挖掘人脸识别所收集到的用户信息的潜在价值，记录顾客男女比例以及年龄阶段和他们分别到店次数，消费时间，分析多次到店及二次消费顾客的购买频率、消费能力等相关信息，对比顾客数据的变化趋势，为经营决策提供数据参考
***
### 人工智能概率性与用户痛点：
* 最小可用产品：VIP定制服务中使用人脸对比功能，基于贵宾定制化服务要求，对于产品的精确度要求相对较高。采用如下方法解决：
1.数据库增添更多的用户图片做训练模型，提高产品的判断准确率
2.人工辅助验证用户信息
ps：资金投入、技术投入要求较低，操作可行性强
* 其他功能：由于个性化套餐、拼桌匹配主要是运用在线人脸搜索功能以及人脸检测与属性分析功能来增加与用户之间的互动满足消费者个性化定制化的消费诉求，因此对于产品的概率性要求相对较低，判错对用户的体验影响较小

### 案例 : 
* 自助点餐（人脸检测与属性分析）
用户在自助点餐机点餐，点餐机将针对用户面部特征的详细分析，判别年龄性别、心情指数、颜值指标等并结合用户订单历史记录，为其推送定制鼓励语和个性化套餐。
* 拼桌匹配（人脸搜索）
当用户选择拼桌服务后，系统将为该时段选择拼桌服务中人脸相似度最高的客户之间进行拼桌配对
* VIP定制服务（人脸对比）【最小可用产品】
当系统通过人脸识别系统检测到VIP用户后，调出该VIP会员的资料，并主动通知监控点的人员进行接待
* 数据屑整理分析
通过人脸识别记录顾客到店次数，分析多次到店及二次消费顾客的购买频率、消费能力等相关信息，对比顾客数据的变化趋势，为经营决策提供数据参考

### 需求列表
 用户案例 | 对应标题 | AI应用
---|--- |--- |
个性化服务 | 心情点餐 | 人脸检测与属性分析 | 
定制化服务 | VIP定制服务 | 人脸对比 | 
个性化服务 | 拼桌匹配 | 人脸搜索 | 
***
### 使用者交互及设计: 
#### 操作流程
[![操作流程.png](https://i.loli.net/2018/12/09/5c0c811c0bf53.png)](https://i.loli.net/2018/12/09/5c0c811c0bf53.png)
#### 产品使用流程图
!产品使用流程图.jpg](https://i.loli.net/2018/12/20/5c1b7353885e6.jpg)
#### 产品框架图
[![功能结构图.png](https://i.loli.net/2018/12/09/5c0c8b326c7c7.png)](https://i.loli.net/2018/12/09/5c0c8b326c7c7.png)
#### axure原型
[![心情点餐](https://i.loli.net/2018/12/09/5c0c63f22795d.png)](https://i.loli.net/2018/12/09/5c0c63f22795d.png)
[![拼桌匹配](https://i.loli.net/2018/12/09/5c0c63f23d3a2.png)](https://i.loli.net/2018/12/09/5c0c63f23d3a2.png)
![微信图片_20181220180458.png](https://i.loli.net/2018/12/20/5c1b6accce777.png)
***
### API展示
功能：心情点餐
服务平台：百度AI
AI产品：人脸检测与属性分析
* http方法：post
* url接口：https://aip.baidubce.com/rest/2.0/face/v2/detect
encoding:utf-8
 --- 
功能：餐桌匹配
服务平台：百度AI
AI产品：人脸搜索
* http方法：post
* url接口： https://aip.baidubce.com/rest/2.0/face/v2/identify
 --- 
功能：VIP定制服务
服务平台：百度AI
AI产品：人脸对比
* http方法：post
* url接口：https://aip.baidubce.com/rest/2.0/face/v2/match
encoding:utf-8
**API CHA



百度AI 定价：
API调用全部免费QPS按照阶梯价格计费，可按天按月灵活购买：最低150元 / 月 / QPS 或 15元 / 天 / QPS
face+++ 定价：
注册免费试用，其余则按量计费（每次调用0.0005元起），按小时计费（每小时5元起）

准确率：国际人脸识别评估集LFW榜， face++ 99.5% , 商汤 99.53% ， 腾讯 99.65% , 百度 99.77%，中科奥森 99.77% , 中科云从 99.5%， 颜鉴99.64%，北京飞搜科技 99.4% ,宇泛智能 99%

次级：EyeKey网站以及虹软技术

测评考虑：识别率以及识别效率

测评网站：（北冥大帝）


#### 问题 Questions: 
* 如何提高图片识别的准确率？
* 系统如何明确图片里用户所指定的主体？
#### 不做 Not doing:
已记录的功能： 人脸识别，人脸认证 ；超出范围的功能：
