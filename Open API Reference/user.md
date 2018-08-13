# 用户接口 #

销售易提供以下接口来管理用户：
* [获取用户接口描述](## 获取用户接口描述)
* [创建用户](## 创建用户)

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


<table border="0.5px" align="center" bordercolor="gray" style="background:gray" width="80%" height="100px" style="font-family:微软雅黑; font-size:14px">
    <tr align="left">
        <th>
    {
    "name": "user",
    "custom": false,
    "label": "用户",
    "disabled": false,
    "createable": true,
    "deletable": true,
    "updateable": true,
    "queryable": true,
    "feedEnabled": true,
    "fields": 
        {<br>
            "propertyname": "id",
            "label": "ID",
            "type": "id",
            "itemType": "long",
            "defaultValue": null,
            "enabled": true,<br>
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

### 描述 ###

创建一个销售易用户。

### URL ###

```Python
https://api.xiaoshouyi.com/data/v1/objects/user/create
```
### HTTP请求方法 ###

POST

### 请求参数 ###

相关字段的权限说明请参见[describe接口说明]()。

### 返回参数 ###

返回错误代码请参见[错误代码说明]()。下表为本接口特有字段说明：

| 返回字段        | 字段类型   |  字段说明 |
| --------   | ----- | ---- |
| id  | long | 新创建的用户ID（唯一标识) | 

### 请求示例 ###

```Python
{
    "record": {
        "email": "xsytest@xiaoshouyi.com",
        "phone": "17798889875",
        "name": "xsy_z",
        "icon": "image",
        "gender": "1",
        "departId": 25314,
        "employeeCode": "077",
        "positionName": "xsy"
    }
}
```

### 返回示例 ###

```Python
{
    "id": 38601
}
```


