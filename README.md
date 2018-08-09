# Open API使用手册

# API简介 #
API（ApplicationProgrammingInterface,应用程序编程接口）是一些预先定义的函数，目的是提供应用程序与开发人员基于某软件或硬件得以访问一组例程的能力，而开发者可以不用关心应用程序内部的实现。

举一个简单的例子，有一个城市A一直没有通电，城市中群众考虑到没有电生活很不便捷，所以向城市B申请，B城市有专门的发电站；B城市经过讨论最终决定由本市的供电局为A城市拉了一根输电线路。但是现在虽然有了电缆，但是并没有接入到A城市；所以A城市的供电局人员需要按照B城市供电局的规范，将输电线路接入到A城市电站，以给市民使用。通过这个例子，A城市可以理解为需要对接的客户，B城市是销售易，B供电局是销售易API研发人员，A供电局是客户的研发人员，电缆便是我们的API。
## 销售易API ##
销售易系统提供了简单、强大、安全的接口能力，方便第三方应用数据和销售易进行集成。
### Open API ###
销售易Open API基于REST API的风格，支持GET、POST操作。
### Bulk API ###
批量 API 是基于 Open API，并对载入或删除大型数据集进行了优化。通过提交批次，您可以使用异步查询、插入、更新、更新插入或删除许多记录。
##接口访问频次限制##
**在使用Open API注意时，请注意以下限制：**

* 每日次数访问限制
  * Open API每日访问次数与购买的API用户数有关，每个租户每日可用用户乘以1000次；假如您购买了100个API用户，那您每日的API访问次数为100*1000=100000次。
* 每秒并发数限制
  *  每个用户在1秒内可调用15次API。

**在使用Bulk API注意时，请注意以下限制：**

* 每天每租户Bulk API请求次数最大300。
* 每秒每租户Bulk API请求次数最大为15。
* 每租户文件上传大小限制20M。
* 每异步任务提交数据量最大为5000。
* 每异步任务查询返回数据量最大为5000。
>_<b style="color:red">NOTE:</b>无论是Open API还是Bulk API都使用了OAuth2.0协议进行安全认证，确保数据的安全访问，认证成功后，开发者可以使用系统分发的Access token对系统内的业务数据进行访问。参考OAuth安全验证[获取Access token]()。具体接口信息请参考[Open API Reference]()和[Bulk API Reference]()。_

## 术语定义 ##

销售易API是通过Https协议以Json格式进行数据交换，接口认证方式采用的是OAuth2.0认证。

|术语|解释说明|
|-|-|
|HTTPS|销售易API是采用Https协议进行数据传输，是安全的加密传输协议。|
|JSON|JSON是一种轻量级的数据交换格式，具有以下特点：<br> 1.格式比较简单，易于读写，格式都是压缩的，占用带宽小;<br>2.易于解析;<br>3.支持多种语言;<br>4.代码开发量较少，易于维护|
|OAuth2.0|OAuth2.0协议认证是主要的用户身份验证和授权方式。<br>为了保证API的访问安全性，所有调用销售易API的开发者都需要完成OAuth2.0协议认证规范，获取到访问令牌(access token)之后才可以调用API|
|接口职能|销售易所提供的API可以是对销售易系统中的一些对象的操作进行的封装，例如：修改客户API，可操作这个接口的用户必须满足：更新客户的功能权限，并且更新的客户必须是未删除、在数据权限范围内的客户等销售易系统规则；否则API调用会提示相应的错误信息。查询等接口同样需满足系统规则。<br>_<b>NOTE:</b> 所以，在确认系统对接需求时，一定要明确此需求在销售易系统中能否执行！_|

# 开始开发 #

如果您是新用户，我们建议您阅读使用手册按照以下顺序：
* 使用销售易API之前需要[开通API License](https://github.com/Doraliudd/OpenAPIGuide/edit/master/apiInstructions/%E5%BC%80%E9%80%9AAPI%20License)。
* 创建连接器是使用OAuth2.0认证的前提条件，您必需先在销售易的后台管理系统[创建连接器](https://github.com/Doraliudd/OpenAPIGuide/blob/master/apiInstructions/createConnector.md)，此连接器与您需要对接的第三方应用程序相关。
* 销售易Open API使用[OAuth2.0安全认证]()来确保数据的安全。
* 销售易Open API通过HTTP协议与用户通信，需要了解[HTTP请求方式]()。


