# 登录

输入手机号、短信验证码完成登录操作

---

**调用地址：**  
待定

**请求参数：**

明文：

```js
{
    phone: "15810430366", //string, require. 登录手机号
    yzm:"8738"//string, require. 短信验证码    
}
```

**返回参数：**

明文：

```js
{
    code: 0000, // int, require. 返回码：0000-成功，-XXXX其他错误标识
    msg: "返回码说明", // string, require, 返回码说明：成功或错误描述
    data:{ 
          user_id:"3211"// 用户Id
          }
}
```

![](/assets/login.png)

