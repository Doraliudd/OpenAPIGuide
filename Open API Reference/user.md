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

/* Pretty printing styles. Used with prettify.js. */
/* Vim sunburst theme by David Leibovic */

pre .str, code .str { color: #65B042; } /* string  - green */
pre .kwd, code .kwd { color: #E28964; } /* keyword - dark pink */
pre .com, code .com { color: #AEAEAE; font-style: italic; } /* comment - gray */
pre .typ, code .typ { color: #89bdff; } /* type - light blue */
pre .lit, code .lit { color: #3387CC; } /* literal - blue */
pre .pun, code .pun { color: #fff; } /* punctuation - white */
pre .pln, code .pln { color: #fff; } /* plaintext - white */
pre .tag, code .tag { color: #89bdff; } /* html/xml tag    - light blue */
pre .atn, code .atn { color: #bdb76b; } /* html/xml attribute name  - khaki */
pre .atv, code .atv { color: #65B042; } /* html/xml attribute value - green */
pre .dec, code .dec { color: #3387CC; } /* decimal - blue  */

pre.prettyprint, code.prettyprint {
    background-color: rgb(47, 54, 64);
    border-radius: 8px;
}

pre.prettyprint {
    display: block;
    width: 95%;
    margin: 1em auto;
    padding: 1em;
    box-sizing: border-box;
    overflow: auto;
}


/* Specify class=linenums on a pre to get line numbering */
ol.linenums { margin-top: 0; margin-bottom: 0; color: #AEAEAE; } /* IE indents via margin-left */
li.L0,li.L1,li.L2,li.L3,li.L5,li.L6,li.L7,li.L8 { list-style-type: none }
/* Alternate shading for lines */
li.L1,li.L3,li.L5,li.L7,li.L9 { }

@media print {
  pre .str, code .str { color: #060; }
  pre .kwd, code .kwd { color: #006; font-weight: bold; }
  pre .com, code .com { color: #600; font-style: italic; }
  pre .typ, code .typ { color: #404; font-weight: bold; }
  pre .lit, code .lit { color: #044; }
  pre .pun, code .pun { color: #440; }
  pre .pln, code .pln { color: #000; }
  pre .tag, code .tag { color: #006; font-weight: bold; }
  pre .atn, code .atn { color: #404; }
  pre .atv, code .atv { color: #060; }
}

body{margin:0;padding:0}
h2{ font-family: 宋体;}
.prettyprint span{
    line-height:21px;
    font-size:18px;
}
pre code{ width:100%; overflow:auto; display:block;}

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
