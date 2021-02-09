---
title: java code 
tags: code,btlord
renderNumberedHeading: ture
grammar_cjkRuby: true
---


---

# 关于查找 <i class="fas fa-coffee"></i>

## 普通查找
```java
    public static int indexof(int[] arr, int target) {
        int res = -1;
        //设置一个最终结果的初始值为-1
        for (int i = 0; i < arr.length; i++) {
        //开始循环
            if (arr[i] == target) {
            //如果相等,使得结果等于索引
                res = i;
                break;
            }
        }
        return res;
    }
    //结果返回target索引
```

## 二分查找

```java

    public static int binarySearch(int[] arr, int target) {
        int begin = 0;      
        //定义起点,也就是左边的游尺
        int end = arr.length - 1;   
        //定义刚刚开始的终点,也就是右边的游尺
        while (begin <= end) {      
        //加入循环,使得左游尺永远小于右游尺,如果擦肩而过,就退出循环
            int indexOfMid = begin + ((end - begin) >> 1);
            //寻找中间索引
            int mid = arr[indexOfMid];
            //寻找中间索引的值
            //接下来,进行判断
            if (target > mid) {         
            //左游尺往右走
                begin = indexOfMid + 1;
            } else if (target < mid) {  
            //右游尺往左走
                end = indexOfMid - 1;
            } else {                    
            //如果和中间值相等,返回找到的索引
                return indexOfMid;
            }
        }

        return -1;
        //如果都没有找到,则返回-1
    }

```





