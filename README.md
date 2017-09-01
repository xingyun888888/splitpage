### splitpage(分页插件)

##### [参考博客](http://www.cnblogs.com/puyongsong/p/6297706.html)

---

#### 快速使用:

1.安装  npm install splitpage

2.配置项opt

``` 
   paginationBox:'',//分页容器(必填)
   mainBox:'',//内容盒子(必填)
   numBtnBox:'',//数字按钮盒子(必填)
   btnBox:'',//按钮盒子(必填)
   ipt:'',//input class(必填)
   goBtn:'',//go btn class(必填)
   currentBtn:'',//当前按钮class name(必填)
   pageCount:1,//每页显示几条数据
   numBtnCount:3,//当前页左右两边各多少个数字按钮
   currentPage:0,//当前页码data-page，首屏默认值
   maxCount:0,//ajax请求数据分成的最大页码
   data:[]//ajax请求的数据
   prevBtnText:"上一页",
   firstBtnText:"首页",
   lastBtnText:"尾页",
   nextBtnText:"下一页",
   confirmText:"确定"   
```
配置参数：  
<table>
    <tr>
        <th>参数</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>opt</td>
        <td>配置项opt</td>
    </tr>
    <tr>
        <td>obj</td>
        <td>后端返回来的数据(数组)</td>
    </tr>
    <tr>
        <td>callback</td>
        <td>切换页面时回调函数,实现自己逻辑</td>
    </tr>
</table>

如何使用:
```   
   function callback(json){
      //实现自己的逻辑代码  
       console.log(json);
   }
   paginationNick({
       paginationBox:'pagination-nick',//分页容器--必填
       mainBox:'main-box-nick',//内容盒子--必填
       numBtnBox:'num-box-nick',//数字按钮盒子-- 必填
       btnBox:'btn-box-nick',//按钮盒子 --必填
       ipt:'page-ipt-nick',//input class-- 必填
       goBtn:'go-btn-nick',//go btn class --必填
       currentBtn:'active-nick',//当前按钮class name --必填
       prevBtnText:"上一页",
       firstBtnText:"首页",
       lastBtnText:"尾页",
       nextBtnText:"下一页",
       confirmText:"确定"
   },obj,callback);

```