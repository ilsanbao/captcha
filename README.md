captcha
=======

golang captcha web server

三个接口：
    
    http://captcha.demo.com/get  
    返回sid与image地址
    
    http://captcha.demo.com/verify 
    传递get接口中返回的sid与用户输入的验证码
    
    http://captcha.demo.com/image 
    直接获取图片，但使用image时，请求verify不需要传递sid。image接口会写sessionCookie
