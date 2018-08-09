# 用户接口 #

销售易提供以下接口来管理用户：
* [获取用户接口描述](##获取用户接口描述)
* [创建用户](##创建用户)

## 获取用户接口描述 ##

### 描述 ###

获取用户对象相关的表结构、数据类型等信息。

### URL ###

```Python
https://api.xiaoshouyi.com/data/v1/objects/user/describe
```
### HTTP请求方法 ###

GET

### 返回示例 ###

tt, code, kbd, samp {
font-family: consolas;
}
.prettyprint, pre.prettyprint {
background-color:#272822;
border:1px solid #272822;
overflow: hidden;
margin:10px0;
font-family:Helvetica,"Hiragino Sans GB","微软雅黑","Microsoft YaHei UI",SimSun,SimHei, arial, sans-serif;
}
.prettyprint.linenums, pre.prettyprint.linenums {
-webkit-box-shadow: inset 40px00#39382E, inset 41px 0 0 #464741;
-moz-box-shadow: inset 40px00#39382E, inset 41px 0 0 #464741;
box-shadow: inset 40px00#39382E, inset 41px 0 0 #464741;
}
.prettyprint.linenums ol, pre.prettyprint.linenums ol {
padding-left:28px!important;
margin:0000px;
}
.prettyprint.linenums ol li, pre.prettyprint.linenums ol li {
padding-left:12px;
color:#bebec5;
line-height:20px;
margin-left:0;
margin:5px;
list-style:decimal;
}
.prettyprint .com {
color:#93a1a1;
}
.prettyprint .lit {
color:#AE81FF;
}
.prettyprint .pun,.prettyprint .opn,.prettyprint .clo {
color:#F8F8F2;
}
.prettyprint .fun {
color:#dc322f;
}
.prettyprint .str,.prettyprint .atv {
color:#E6DB74;
}
.prettyprint .kwd,.prettyprint .tag {
color:#F92659;
}
.prettyprint .typ,.prettyprint .atn,.prettyprint .dec,.prettyprint .var{
color:#A6E22E;
}
.prettyprint .pln {
color:#66D9EF;


<table border="0.5px" align="center" bordercolor="gray" background="gray" width="90%" height="100px" style="font-family:微软雅黑; font-size:14px">
    <tr align="left">
        <th>{
    "name": "user",
    "custom": false,
    "label": "用户",
    "disabled": false,
    "createable": true,
    "deletable": true,
    "updateable": true,
    "queryable": true,
    "feedEnabled": true,
    "fields": [
        {
            "propertyname": "id",
            "label": "ID",
            "type": "id",
            "itemType": "long",
            "defaultValue": null,
            "enabled": true,
            "createable": false,
            "updateable": false,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 100,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "email",
            "label": "邮箱",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 100,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "phone",
            "label": "手机号",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 200,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "unionId",
            "label": "联合认证ID",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 200,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "name",
            "label": "姓名",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": true,
            "sortable": false,
            "minLength": 0,
            "maxLength": 20,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "status",
            "label": "用户状态",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": false,
            "updateable": false,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 4,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "statusInt",
            "label": "用户状态编码",
            "type": "select",
            "itemType": "Long",
            "defaultValue": null,
            "enabled": true,
            "createable": false,
            "updateable": false,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 4,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [
                {
                    "label": "未激活",
                    "value": "0"
                },
                {
                    "label": "已激活",
                    "value": "1"
                },
                {
                    "label": "已删除",
                    "value": "-10"
                },
                {
                    "label": "已离职",
                    "value": "-11"
                }
            ],
            "checkitem": []
        },
        {
            "propertyname": "joinAtStr",
            "label": "入职日期",
            "type": "date",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 10,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "birthday",
            "label": "出生日期",
            "type": "date",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 10,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "employeeCode",
            "label": "员工编号",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 20,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "positionName",
            "label": "职位",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 30,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "userManagerId",
            "label": "主管",
            "type": "reference",
            "itemType": "long",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 20,
            "dependentPropertyName": null,
            "referTo": {
                "label": "用户",
                "belongId": 70
            },
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "gender",
            "label": "性别",
            "type": "select",
            "itemType": "Long",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 4,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [
                {
                    "label": "男",
                    "value": "1"
                },
                {
                    "label": "女",
                    "value": "2"
                }
            ],
            "checkitem": []
        },
        {
            "propertyname": "rankId",
            "label": "职级",
            "type": "select",
            "itemType": "Long",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 20,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [
                {
                    "label": "二级",
                    "value": 899804,
                    "dependentValue": [],
                    "disabled": false
                },
                {
                    "label": "三级",
                    "value": 936571,
                    "dependentValue": [],
                    "disabled": false
                },
                {
                    "label": "一级",
                    "value": 1172174,
                    "dependentValue": [],
                    "disabled": false
                }
            ],
            "checkitem": []
        },
        {
            "propertyname": "languageCode",
            "label": "languageCode",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": false,
            "updateable": false,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 10,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "timezone",
            "label": "timezone",
            "type": "text",
            "itemType": "String",
            "defaultValue": null,
            "enabled": true,
            "createable": false,
            "updateable": false,
            "required": false,
            "sortable": false,
            "minLength": 0,
            "maxLength": 200,
            "dependentPropertyName": null,
            "referTo": {},
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        },
        {
            "propertyname": "departId",
            "label": "部门",
            "type": "reference",
            "itemType": "long",
            "defaultValue": null,
            "enabled": true,
            "createable": true,
            "updateable": true,
            "required": true,
            "sortable": false,
            "minLength": 0,
            "maxLength": 20,
            "dependentPropertyName": null,
            "referTo": {
                "label": "部门",
                "belongId": 50
            },
            "joinTo": {},
            "selectitem": [],
            "checkitem": []
        }
    ],
    "entityTypes": []
}</th>
    </tr>
</table>


## 创建用户 ##
