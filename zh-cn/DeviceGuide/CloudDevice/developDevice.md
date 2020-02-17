### 设备开发 

通过“功能集配置”页面配置好产品的功能后，点击【保存】按钮，进入“设备开发”页面。  


“设备开发”页面主要包括三个信息项，即“开发流程”、“参数配置”、“业务功能”。  

**开发流程：**  

平台提供程序开发需要的开发文档，程序调试工具，在线测试工具。    

![开发流程][Development_process]    

在线测试工具，用于协助验证协议适配是否准确、可用。进入某设备的调试页面后，会看到该设备可以支持调试的单命令、高级命令(即组命令)。这些命令参见《U+开放平台XXX设备功能模型》即`程序开发-开发文档中。

选择相应的功能，点击其【发送命令】操作，日志里即可得到该功能的调试结果。  


<font color="#FF0000">注：请在成功配置设备入网20分钟内点击启动按钮，开始在线测试</font>  

![在线测试工具][Testing_tools] 


**参数配置：**   

平台会自动分配各开发环境需要的SystemID、SystemKey，校验云设备的凭证；  
查询设备信息回调URL，由第三方开发者填写，平台通过本URL来主动向第三方云服务定期同步设备信息；  
读设备属性回调URL，由第三方开发者填写，平台回调本URL通过第三方云服务发送给设备执行，读取设备属性；  
写设备属性回调URL，由第三方开发者填写，平台回调本URL通过第三方云服务发送给设备执行，写设备属性即单命令操作；  
设备操作回调URL，由第三方开发者填写，平台回调本URL通过第三方云服务发送给设备执行，操作设备即组命令操作；
填写好回调URL后，点击【保存】按钮。  

![参数配置][Parameter_configuration]  


开发者在自有云中，需要完成U+ IOT协议和开发者硬件自有协议之间的转换适配，进而实现控制指令由开发者自有智能云下发给设备后可以正确执行。

开发者在自有智能云上需要实现的与平台对接的接口请详见[《接口使用文档》][Dev_world]。

**业务功能：**     

业务上对组命令中各属性值的要求，如有需要添加即可，如无法添加请联系海极网同事。

 
![业务功能][Business_functions]






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
[Business_functions]:_media/Link/Business_functions.png 