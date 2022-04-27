# 软件需求工程与UML建模APP
## 一、最终效果展示

![系统首页.png](https://s2.loli.net/2022/04/26/ZAxuiPsVLkvCKTF.png)  ![教务管理.png](https://s2.loli.net/2022/04/26/msOTIyfbGjcRuK9.png)
![事务管理.png](https://s2.loli.net/2022/04/26/acxMtRw3iYEnoAr.png)  ![实时监测.png](https://s2.loli.net/2022/04/26/tP7Ia5YNOdRjMJn.png)

## 二、结构化需求分析

### 2.1 系统架构图

![系统架构.png](https://s2.loli.net/2022/04/26/MTzDyS72BGe6Qbw.png)

### 2.2 功能分析

**系统目的**：建设建设北京理工大学数据中台，打造集数据采集、数据处理、监测管理、可视化于一体的数据中台。
**功能顶层**：教务管理、学生事务、校园论坛、校园检测。
**基本功能**：

- 教务管理：利用app平台，对接乐学、延河课堂等平台；对接教务管理中心课程表查看、考试安排查看等模块。
- 学生事务：利用app平台，对接请假销假、场地预约平台。
- 校园论坛：实现校内跳蚤市场功能，提供一个校园内部二手交易平台；实现线上论坛功能，提供一个校园互动平台；实现匿名树洞功能，提供一个匿名交流平台。
- 校园监测：提供检测页面，实现实时查看校园中个地点的最新人数的功能。

### 2.3 需求细化与优先级划分

| 涉众                                                         | 主要目标                                                     | 主要关注点                           | 优先级 | 风险评估 |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------ | ------ | -------- |
| 学生                                                         | 能够利用智慧校园管理系统实现实时的信息查询、论坛交流、校园状态查询 | 使用要简单，功能要保证实时性与准确性 | 3      | 高       |
| 老师                                                         | 能够利用智慧校园管理系统实现实时的师生互动以及更便捷的校园设施使用 | 在保证不出差错的情况下提升工作的效率 | 2      | 高       |
| 系统管理员                                                   | 能够利用智慧校园管理系统更方便地管理校园信息                 | 提升管理的效率                       | 1      | 低       |
| ## UML数据建模                                               |                                                              |                                      |        |          |
| - **DFD图-上下文图**                                         |                                                              |                                      |        |          |
| ![上下文图.png](https://s2.loli.net/2022/04/26/anEjOyU7Pegrulq.png) |                                                              |                                      |        |          |
| - **DFD图-0层图**                                            |                                                              |                                      |        |          |
| ![0层图.png](https://s2.loli.net/2022/04/26/7uRKhfZUGEYe3lF.png) |                                                              |                                      |        |          |
| - **DFD图-1层图**                                            |                                                              |                                      |        |          |
| ![1层图.png](https://s2.loli.net/2022/04/27/amFyYPztTUsSIi3.png) |                                                              |                                      |        |          |
| ![事务1层.png](https://s2.loli.net/2022/04/27/UYelRrnozFpAaTi.png) |                                                              |                                      |        |          |
| ![教务1层.png](https://s2.loli.net/2022/04/27/dMUKFGlapu7nLAW.png) |                                                              |                                      |        |          |
| - **实体关系图（ERD）**                                      |                                                              |                                      |        |          |
| ![erd.png](https://s2.loli.net/2022/04/26/No6BdHy8v9EkleT.png) |                                                              |                                      |        |          |
| - **Use Case用例图**                                         |                                                              |                                      |        |          |
| ![use-case-学生.png](https://s2.loli.net/2022/04/26/uq5cFKeTnVD1WUO.png) |                                                              |                                      |        |          |
| ![use-case-老师.png](https://s2.loli.net/2022/04/26/CnlXb6MzN1FdVJk.png) |                                                              |                                      |        |          |
| ![use-case-管理员.png](https://s2.loli.net/2022/04/26/gDvuTnZQrxCB9m4.png) |                                                              |                                      |        |          |
| - **类图**                                                   |                                                              |                                      |        |          |
| ![类图.png](https://s2.loli.net/2022/04/26/u517ypSxVijhFlW.png) |                                                              |                                      |        |          |
| - **顺序图**                                                 |                                                              |                                      |        |          |
| ![注册顺序图.png](https://s2.loli.net/2022/04/26/pOKyqXfHFud7YoE.png) |                                                              |                                      |        |          |
| ![教务管理顺序图.png](https://s2.loli.net/2022/04/26/4J7Brem6kb2TtD3.png) |                                                              |                                      |        |          |
| ## 各模块及详细功能                                          |                                                              |                                      |        |          |
| ### 登录模块                                                 |                                                              |                                      |        |          |
| 为全校师生提供一个简洁的登录界面，同时兼具用户注册、找回密码等功能。师生可通过实名验证提高账号的安全性，大幅度提升个人隐私的安全保障。 |                                                              |                                      |        |          |
| ### 教务管理模块                                             |                                                              |                                      |        |          |
| 教务管理模块为全校师生提供功能完备的教务管理系统，包括乐学、延河课堂、考试安排、课程表等四个模块。乐学为教师和学生提供了远程互动的平台，教师可以在乐学进行教学任务的发布、上传课件、安排课堂作业等任务，学生可以登录乐学进行课件的下载、作业的提交。延河课堂可以自动录制老师的上课视频，学生可以在课后登录延河课堂复习课堂内容，更好地理解课业知识。课程表可以为学生提供课表查询功能，便于学生在短时间内获取最新的课表信息。考试安排将带有自动提醒功能，当教务处上传考试信息后学生和老师能够在第一时间获得考试信息，以便更好地进行教学任务的推进。教务管理模块为智慧校园管理系统的主流信息管理模块，有利于推进教学事务的数字化。 |                                                              |                                      |        |          |
| ### 事务管理模块                                             |                                                              |                                      |        |          |
| 事务管理模块为全校师生提供功能完备的校园事务管理系统，包含请假销假和场地预约的功能。考虑到现实生活中学生前往辅导员办公室请假销假的繁琐步骤，线上的请假销假功能使得学生能够在不受时空限制的情况下更为便利地进行请假销假活动的进行。辅导员可以定期登录请假销假系统进行学生事务的处理，更好地对学生进行管理。线上的场地预约功能便于学生随时随地地进行社区空间和教室的预约，节约了学生在空间上耗费的时间。请假销假和场地预约功能均具有实时提醒功能，便于使用者在第一时间获取相关的事务信息，能够大幅提高校园事务的处理效率，便利全校学生的校园生活。 |                                                              |                                      |        |          |
| 论坛模块为全校学生提供安全可靠的学生论坛系统，提供跳蚤市场，资讯交流，匿名树洞等功能，有利于促进学生之间的信息交流，满足学生的社交需求。 |                                                              |                                      |        |          |
| 目前学校的信息渠道多而繁杂，信息质量良莠不齐，而信息的监管一直是一个令人感到头疼的问题。其中最大的问题是信息的真实性，为了解决这个问题，本项目参考微信小程序“offershow”（薪资查询平台），加入可信度机制。对于某条信息，若用户认为可信，可点击“可信”按钮；认为不可信则点击“不可信 ”，信息默认按照 可信数/不可信数 的顺序排序（也可以手动改成按发布时间排序），这样，就利用了用户自身，实现了信息真实性的监管。 |                                                              |                                      |        |          |
| 跳蚤市场为学生提供了一个二手交易的平台，学生可将自己的闲置物品信息上传至跳蚤市场中拍卖，有购买意向的学生可以点击卖家信息，进行双方的线上交易，在线下约定时间地点自行交易。同时学校也可设定二手交易的监管组织，学生可在论坛上传物品信息后将物品委托给监管组织，由二手组织负责后续物品的交易操作，从而达到节约学生交易时间的目的。 |                                                              |                                      |        |          |
| 咨询交流平台为同学们提供了一个信息交流的平台，学生可在平台上分享学习、生活的信息，进行合理的交流，拓展学生的交友渠道。 |                                                              |                                      |        |          |
| 匿名树洞中的用户昵称均为匿名形式，保障了用户的个人隐私，用户可以在匿名树洞中分享一些私人问题，与其他用户进行更进一步的交流。同时匿名树洞中还含有监控机制，以防止用户发布不良言论。 |                                                              |                                      |        |          |
| 论坛模块的设置增加了学生之间的互动，拓宽了学生的交友空间，丰富了学生的校园生活。 |                                                              |                                      |        |          |
| ### 校园实时状态监测模块                                     |                                                              |                                      |        |          |
| 为全校师生提供校园实时状态监测系统，利用计算机视觉算法监测食堂、超市人流，停车场车数量等信息，有利于防止校园堵塞现象出现，提高使用者的时间利用效率与出行体验。 |                                                              |                                      |        |          |
| 计算机视觉算法方面，采用YOLOv5+DeepSORT作为核心网络模型。利用YOLOv5实现目标检测后，再用DeepSORT对每个目标分配标签，并加入计数线，目标穿过计数线后自动计数。 |                                                              |                                      |        |          |
| 算法工作流程如下：                                           |                                                              |                                      |        |          |
| YOLOv5检测得到boundingbox → 生成detections → 卡尔曼滤波预测 → 使用匈牙利算法将预测后的tracks和当前帧中的detecions进行匹配（级联匹配和IOU匹配） → 卡尔曼滤波更新 → 标签穿过计数线后更新person_in和person_out的数值，person_all = person_in - person_out |                                                              |                                      |        |          |
| 模型训练方面，已完成了行人检测模型的训练。数据集采用Market - 1501开源行人数据集，该数据集在清华大学校园中采集，夏天拍摄，在 2015 年构建并公开。它包括由6个摄像头（其中5个高清摄像头和1个低清摄像头）拍摄到的 1501 个行人、32668 个检测到的行人矩形框。每个行人至少由2个摄像头捕获到，并且在一个摄像头中可能具有多张图像。训练集有 751 人，包含 12，936 张图像，平均每个人有 17.2 张训练数据；测试集有 750 人，包含 19，732 张图像，平均每个人有 26.3 张测试数据。3368 张查询图像的行人检测矩形框是人工绘制的，而 gallery 中的行人检测矩形框则是使用DPM检测器检测得到的。该数据集提供的固定数量的训练集和测试集均可以在single-shot或multi-shot测试设置下使用。在该训练集下，训练集上的准确率到达了98%，测试集中的准确率到达了85%。 |                                                              |                                      |        |          |
| 摄像头调用方面，采用opencv-python库函数，实现了摄像头的调用。 |                                                              |                                      |        |          |
| 与后端服务器的交互方面，采用txt文本与服务器交互。检测模型实时检测各食堂、超市等地的人数并写入txt文档，服务器每隔5秒从txt文件中读取各地人数并更新，供师生查看。 |                                                              |                                      |        |          |
| ## 团队成员及分工                                            |                                                              |                                      |        |          |
| 成员                                                         | 工作                                                         |                                      |        |          |
| ---                                                          | ---                                                          |                                      |        |          |
| 郑乐祺                                                       | 完成整个项目的统筹工作，负责APP中登录注册模块的实现，完成APP与数数据库的连接，负责代码仓库的构建，负责需求文档的部分编写 |                                      |        |          |
| 林宏鹏                                                       | 负责APP界面中教务管理模块的界面实现，完成APP与数据库的连接，负责代码仓库的构建，负责需求文档的部分编写 |                                      |        |          |
| 李赛伽                                                       | 负责APP界面中论坛模块的设计与实现，负责博客的编写与上传，负责需求文档的部分编写 |                                      |        |          |
| 余力                                                         | 负责APP界面中实时监控模块的界面实现，负责需求文档的部分编写  |                                      |        |          |
| 郑路洁                                                       | 主负责需求文档的撰写，负责计算机视觉模型的训练与部署，APP界面设计 |                                      |        |          |
| 张博涵                                                       | 主负责需求文档的撰写，负责APP界面的设计，负责代码的测试      |                                      |        |          |
| ## 团队工作                                                  |                                                              |                                      |        |          |
| - **第一周**：确认项目主题为智慧校园数据管理系统，与甲方小组进行面谈沟通，获取项目的具体需求，完成项目的需求分析，确认系统的核心功能，确定未来几周的时间安排，以及人员分工，建立Github仓库，完成系统结构图。 |                                                              |                                      |        |          |
| - **第二周**：按照第一周拟定的人员分工，完成初步主界面设计文档与UI设计，学习安卓和数据库的相关技术，编写软件需求规格文档。 |                                                              |                                      |        |          |
| - **第三周**：进行安卓界面的编写代码，基本完成App中登录注册、数据管理、实时监控等核心功能，学习数据库相关知识，开始建立本地数据库，编写软件需求规格文档。 |                                                              |                                      |        |          |
| - **第四周**：完成app剩余核心功能中的论坛模块，完成数据与安卓系统的连接，完成软件需求规格文档，将代码放入仓库。 |                                                              |                                      |        |          |
| - **第五周**：对系统的整体界面进行修改，对系统进行测试，修补系统中的不足，完成整个项目的总结与分析，准备课堂最后的汇报工作。 |                                                              |                                      |        |          |

## YOLOV5+DeepSORT部分
由于文件过大，故放入百度网盘
链接：https://pan.baidu.com/s/1KdFQBTLoVa-o9l3zwWIZDA 
提取码：1234
提取后，在yolov5-deepsort路径下终端运行`pip install requirements`配置环境，配置好后运行count_person.py即可
目前已成功调用摄像头，并且会把 监测人数+150 写入person_count.txt，供后端服务器读取

