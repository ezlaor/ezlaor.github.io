
# 我的UI工作小结(Vue.js+ElementUI)

## 引言
   小组分工明确非常重要，不过这也同时意味着每个人必须尽到充分的输出，
这学期我在项目中担任**UI**（``UI``的全称是'用户接口（``User Interface``）'，至此我对这个称谓已有所体会…）。
UI这个位置很神秘，好的UI可以让有所欠缺的项目得到表现，失败的UI会让一个**非常优秀**的项目失去优势……~~（是我的锅）~~，

## 开始工作
  我的想法是UI在每一轮迭代中应该最先搭建好``html``布局并在代码合并后调整``css``参数，这样前端其他成员才方便进行``js``脚本
编码和后端服务对接等任务，之后再参与测试和其他多项任务的编码。我在项目开发中写``html``时就会发现：
使用表单标签``<form></form>``比一个个把``<input>``放进``<div></div>``要科学得多，又或者在``css``里面设置``width``或``height``到底是
百分比好还是设置``px``、``rem``好…

## 0.和产品经理商量原型
   我觉得软件项目的不确定性就在于此，如果看不到原型相信凭空设计一个页面对UI设计者来说会非常困难，因为原则上绝不能违背需求，
UI设计不能凭主观审美来驱动。原型设计可以帮助UI了解到这个页面需要操作的具体数据和必须展示的必要栏目，同时一些页面跳转等非常
重要的交互逻辑需要提前考虑清楚。
 
### 1.考虑第三方组件库
 
 - [iView](http://v1.iviewui.com/)
    
 - [Element](https://element.eleme.cn/#/zh-CN/component/installation)
   
   原生的``html``标签渲染得到的组件真的不好看，对一个需要强调用户体验和实际功能的产品不太友好，有些组件库
  自带的主题或内置的响应信息非常完善，会减轻很多前端压力，辅助敏捷开发。
  iView和elementUI都是轻量级、易于web网站快速成型的桌面端组件库，我们小组用的是Element(其实组员都觉得Element的设计
  更切合移动端。 ~~还是我的锅~~)
  
### 2.尝试一个布局 
 
 ~~~python
#!/html

<!DOCTYPE html>
<html>
<head>
<style>
#header {
    background-color:#00b38a;
    color:white;
    text-align:center;
    padding:5px;
}
#nav {
    line-height:30px;
    background-color:#eeeeee;
    height:300px;
    width:100px;
    float:left;
    padding:5px;	      
}
#section {
    width:350px;
    float:left;
    padding:10px;	 	 
}
#footer {
    background-color:#eeeeee;
    color:white;
    clear:both;
    text-align:center;
   padding:5px;	 	 
}
</style>
</head>

<body>
<div id="header">
<h1>我的布局</h1></div>

<div id="nav">
选项一<br>
选项二<br>
选项二<br>
</div>

<div id="section">
<h2>Demo</h2></div>

<div id="footer">
联系我们</div>

</body>
</html>

~~~
![](image/html1.png)

 


