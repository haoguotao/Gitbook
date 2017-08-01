# 首页

获取首页展示的产品信息，按照类别分为：热门、所有

**调用地址：**  
待定

**请求参数：**

明文：

```js
{
    type: 1, //int, require. 类型定义：1-热门产品，2-所有产品    
}
```

**返回参数：**

密文：

```js
{
    code: 0000, // int, require. 返回码：0000-成功，-XXXX其他错误标识
    msg: "返回码说明", // string, require, 返回码说明：业务数据：返回code非0时才有
    data:{ // jeson object, require, 业务数据：返回code非0时才有
          list:[{
            id: "3",
            name: "\u8fd0\u8425\u5546\u8ba4\u8bc1",//产品名称
            img_url:”logo地址”,       //
            tag : [”三分钟审核”,”利率低”,”有身份证即可”],
            rate : “98%”,             //通过率
            Repayment : [1,34],       //还款期限 1-34 个月
            Loan_limit : [500,10000], //贷款额度 500-10000 
                statu": 1,                //  1为显示  2为隐藏
            }, 
                {
             id: "2",
             name: "\u829d\u9ebb\u5206\u8ba4\u8bc1",
             tag : [”三分钟审核”,”利率低”,”有身份证即可”],
             img_url:”logo地址”,
             status: "1" // 1为显示  2为隐藏
                }]
}
```



