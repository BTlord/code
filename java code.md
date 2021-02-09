---
title: java code record
tags: code,btlord
renderNumberedHeading: ture
grammar_cjkRuby: true
---


---

# 二分查找 <i class="fas fa-coffee"></i>
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
```




