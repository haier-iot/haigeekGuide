####  定义产品功能集    

> 对于各品类的产品，平台已制定了标准的产品功能定义即功能集又称功能模板；且对于标准的功能定义，小优音箱也在语义层面支持语音控制。
产品功能定义，描述了产品具有哪些功能，包括基础功能、高级功能、告警、其他功能。 本文截图以创建智能灯具为例。  


概念|解释
:-|:-
基础功能|单一的功能操作即属性，属性支持被查询、控制和订阅，如灯的开关
高级功能|主要用于向设备下发组合控制指令，该功能即可以定义为方法，方法可支持同时下发多个属性（参数），如电灯的模式及亮度
告警|主要用于设备向云端上报组合数据，可支持同时上报多个属性（参数），如洗衣完成
其他功能|主要用于设备向云端上报组合数据，可支持同时上报多个属性（参数），服务大数据 

<font color="#FF0000">注：高级功能，平台默认需要实现的组命令：getAllProperty(查询所有属性)、getAllAlarm(查询报警)、stopCurrentAlarm(停止报警)</font>

##### 功能集添加 

通过“创建功能集”点击【确定】按钮后会弹出“产品选择功能”对话框页面，选择相应的功能模板，选择产品要实现的功能，点击【添加选中功能】按钮。  


![云设备功能集定义][Function_set]


##### 功能集配置  


通过【添加选中功能】进入“功能集配置”页面，可按照标准或自定义配置产品的功能。

平台会根据产品的类型默认配置好标准功能（可点击图中【标准服务】按钮查看）。默认配置的标准功能包括必选和非必选，开发者可通过【自定义功能】来自定义增添新的功能，高级功能信息项不支持自定义，开发者也可对部分功能并进行编辑。   

<font color="#FF0000">注：自定义功能不支持接入高级服务（如U+APP、场景……）如需要新增或修改标准功能，请联系标准团队进行功能标准化(wangxianqing.uh@haier.com)</font>  

在产品最终上线前，功能定义的状态会保持“开发中”，该状态下可随时调整功能定义。一旦产品开始提交上线申请或已上线，状态会随之改变为“审核中”或“已上线”，之后功能定义不可再修改。

![基础功能][Basis_function]  

![高级功能][Advanced_function]

![其他功能][Other_function]


**基础功能信息项说明：**  
支持自定义功能  

信息项|说明|备注
:-|:-:|:-
序号|即所选功能的顺序号，通讯协议按此序号生成|无
显示名称|属性的说明|无
标识名称|即属性名称|添加自定义功能时，建议格式为"第三方标识字母_"，例如，“haier_”
读写类型|包括：读、写、单可写、组可写|无
数据类型|包括：整型、布尔、字符串、浮点型、时间、枚举等|无
属性位置|表示某个已定义的属性在字节中的位置|无
取值描述|属性的数据类型描述|无
指令|E++协议负载指令|无
操作|包括：修改、重置(更新)、删除、上移、下移|可修改取值描述



**高级功能信息项说明：**  
不支持自定义功能  

信息项|说明|备注
:-|:-:|:-
序号|即所选功能的顺序号，通讯协议按此序号生成|无
命令名称|组命令操作名称|无
指令|E++协议负载指令|无
输入参数/属性位置|表示某个已定义的属性在组命令中的字节位置|无
操作|包括：修改、删除|默认实现的组命令不可操作


**告警功能信息项说明：**  
支持自定义功能，主要用于设备向云端上报。  

信息项|说明|备注
:-|:-:|:-
序号|即所选功能的顺序号，通讯协议按此序号生成|无
显示名称|组命令操作名称|无
标识名称|即属性名称|添加自定义功能时，建议格式为"第三方标识字母_"，例如，“haier_”
数据类型|包括：整型、布尔、字符串、浮点型、时间、枚举等|无
操作|包括：修改、重置(更新)、删除、上移、下移|可修改取值描述 


**其他功能信息项说明：**  
支持自定义功能 ，主要用于设备向云端上报。 

信息项|说明|备注
:-|:-:|:-
序号|即所选功能的顺序号，通讯协议按此序号生成|无
显示名称|属性的说明|无
标识名称|即属性名称|添加自定义功能时，建议格式为"第三方标识字母\_"，例如，“haier\_”
读写类型|包括：读、写、单可写、组可写|无
数据类型|包括：整型、布尔、字符串、浮点型、时间、枚举等|无
大数据属性位置|表示某个已定义的属性在字节中的位置|无
取值描述|属性的数据类型描述|无
操作|包括：修改、重置(更新)、删除、上移、下移|可修改取值描述





[Access_plan]:_media/Link/guide.png  
[Architecture]:_media/Link/architecture.png 
[Create_function]:_media/Link/create_function.png  
[Create_function2]:_media/Link/create_function2.png  
[Function_set]:_media/Link/function_set.png  
[Haigeek]:https://www.haigeek.com/web/pages/haigeek.html
[Basis_function]:_media/Link/basis_function.png 
[Advanced_function]:_media/Link/advanced_function.png 
[Other_function]:_media/Link/other_function.png
[Development_process]:_media/Link/development_process.png
[Parameter_configuration]:_media/Link/parameter_configuration.png  
[Product_model]:_media/Link/product_model.png 
[Create_model]:_media/Link/create_model.png  
[Create_success]:_media/Link/create_success.png 
[Create_model]:_media/Link/model_success.png  
[AccessU+]:_media/Link/accessU+.png 
[App_config]:_media/Link/app_config.png  
[Click_config]:_media/Link/click_config.png   
[U+_ui]:_media/Link/u+_ui.png    
[Scene_function]:_media/Link/scene_function.png 
[Expand_functionality]:_media/Link/expand_functionality.png
[Dev_world]:https://haier-iot.github.io/guide/#/zh-cn/Cloudgw  
[Testing_tools]:_media/Link/testing_tools.png 
[Online_apply]:_media/Link/online_apply.png 
[Submit_audit]:_media/Link/submit_audit.png 