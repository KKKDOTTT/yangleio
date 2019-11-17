# yangleio
字符串实验
==========
实验目的
--------
1、掌握字符串String及其方法的使用<br>
2、掌握异常处理结构<br>

实验内容
--------
内容：利用已学的字符串处理知识完成《长恨歌》古诗的整理对其工作，写出功能函数，并运行。达到如下功能：<br>
1、每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”<br>
2、允许提供输入参数，统计古诗中某个汉字或词出现的次数。<br>
3、考虑操作中可能出现的异常，在程序中设计异常处理程序。<br>

实验步骤
-------
1、编写主函数调用tianjia函数和chazhao函数<br>
2、编写tianjia子函数<br>与chazhao子函数<br>


核心代码
--------
```
public static StringBuffer Tianjia(StringBuffer str) {
  StringBuffer str1=new StringBuffer();
  for(int i=0;i<str.length()/7;i++){
    str1.append(str.substring(7*i,7*(i+1)));
    if((i+1)%2!=0){
     str1.append("，");
    }
    else{
     str1.append("。").append("\n");
    }
  }
  return str1;
}
```
添加“，”“。”的子函数Tianjia<br>
利用所学的for循环编写一个if条件的函数，如果如果句数为奇数加逗号，反之则加句号。 <br>
```
public static int Chazhao(String orgstr,String findstr){
 int x=0;
 while(orgstr.indexOf(findstr)!=-1){
  if(orgstr.indexOf(findstr)!=-1){
   x++;
   orgstr=orgstr.substring(orgstr.indexOf(findstr)+findstr.l
  ```
查询字词数量的子函数Chazhao<br>
定义整型x参数并初始化x=0
利用`indexOf`在字符串中搜索字符或子串，返回查找对象首次在字符串中出现的位置，如果没有返回-1<br>
利用`if`如果`indexOf`返回的值不等于-1则`x++`<br>

实验结果
-------
![](https://github.com/Listen-lei/-/blob/master/1.PNG)</div>

感想
----
还需多加练习。
