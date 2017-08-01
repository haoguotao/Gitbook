# 产品详情页

获取展示的产品详细信息

---

**调用地址：**  
待定

**请求参数：**

明文：

```js
{
    id: 1, //int, require. 产品id
}
```

**返回参数：**

明文：

```js
{
    code: 0000, // int, require. 返回码：0000-成功，-XXXX其他错误标识
    msg: "返回码说明", // string, require, 返回码说明：成功或错误描述
    data:{ // jeson object, require, 业务数据：返回code非0时才有
            id: "2",
            name: "\u829d\u9ebb\u5206\u8ba4\u8bc1",
            img_url: "logo地址", 
            Repayment : [1,34],  还款期限 1-34 个月
            Loan_limit : [500,10000], 贷款额度 500-10000 
            Condition : “申请条件”,
            Auth : “官网认证”,
            Tag : [”急速小额”,”最高可借”,”快速审核”,”超低利率”,”0抵押”],
            Information : [“二代身份证”,”手机运营商授权”,”信用卡实名认证”]
            }
}

```



