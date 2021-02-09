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
        for (int i = 0; i < arr.length; i++) {
            if (arr[i] == target) {
                res = i;
                break;
            }
        }
        return res;
    }
    //结果返回target索引
```

## 二分查找






