# ARegisterPage
===========================
这个是开始接触表单的时候开始写的一个静态页面，不过表单内容剧多，也遇到了不少问题，刚开始方法也比较笨，不过还是放上来瞅瞅。主要还是问题吧，说不定以后还能造福初学者呢。

===========================
1. 表格文字被设置成漂亮的华文行楷，在别人的浏览器上竟然不识别，原因是不是所有人的系统都装有华文楷体。
* 表格里分别设置两列的属性，可以使用如下形式  
table tr td:nth-child(1) {  
    text-align: right;  
}  

table tr td:nth-child(2) {  
    text-align: left;  
    color: blue;  
}  
* 提示框里的value不要用来显示提示性文字，而要用placeholder

##<a name="code"/>
```javascript
表格中复选框要写<label></label>:    
```  
```javascript  
 <input type="checkbox" value="小学数学">小学数学     
```  
要写成：  
```javascript  
 <input type="checkbox" value="小学数学"><label>小学数学</label>     
```  

或者写成   
```javascript  
 <input type="checkbox" value="小学数学" id="math"><label for="math">小学数学</label>    
```  
 
===========================
节目预告：哈哈，明天放个十字架，用到了盒模型。另外mark一些垂直居中方法吧~:astonished:
