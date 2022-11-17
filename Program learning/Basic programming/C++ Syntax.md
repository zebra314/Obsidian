---
tags: programming, competitive_programming, c++ 
---

# ```set``` , ```multiset```

1. STL容器
2. ```.insert()```插入元素
3. ```set```會自動消除重複元素, ```multiset```會保留
4. 元素插入後會自動排序
5. ```.clear()```初始化
6. ```.earse()```刪除指定元素
7. ```.count()```判斷元素是否存在,回傳 0 or 1
8. ```.find()```也是用來判斷元素是存在,但回傳的是指向其儲存位址的指標

# ```lower_bound()``` ,  ```upper_bound()```

1. ```lower_bound(``` _.begin()_ ```,``` _.end()_ ```,``` _value_ ```)```
2. 返回數值  
3. Binary Search
4. ```*lower_bound()``` 指向該數值的儲存位置
5. 可用來取代數值

# ```find()```

1. 檢查, 搜尋位置
2. 返回位址
3. Code:

```c
 auto it = find(v.begin(), v.end(), K);

    // If element was found
    if (it != v.end())
    {
        // calculating the index
        // of K
        int index = it - v.begin();
        cout << index << endl;
    }
    else {
        // If the element is not
        // present in the vector
        cout << "-1" << endl;
    }
```

# ```.end()```  ```.back()```  ```.front()```  ```.begin()``` 差別

```c
v: [ 1 | 2 | 3 | 4 | ... | 999 ]
     🡑                      🡑     🡑
   front()                back() end()
     🡑
   begin()
```

# ```isalpha()```  , ```isdigit()```

+ 用來判斷字元是字母或數字
+ 回傳bool

```c
isalpha('a') == 1
isalpha('1') == 0
isdigit('a') == 0
isdigit('1') == 1
```

# ```.length()``` ,  ```.size()```

+ 回傳int

```c
a.length()
a.size()
```

# ```Vector``` 更動元素 

+ ```.erase()``` 刪除特定位置

    ```c
    b.erase(b.begin()+3); //刪除第三個元素(b[2])
    b.erase(b.begin()+3,b.begin()+6); //刪除第三到第六個元素
    ```

+ ```.insert()``` 新增至特定位置

    ```c
    b.insert(b.begin(),element); //在開頭加入element
    ```

# ```float``` ,  ```double``` 差別

+ ```float``` 32位元 有效數字6~7
+ ```double``` 64位元 有效數字15~16 (比較精確)  

# ```cin``` ,```cout``` 優化

```c
ios::sync_with_stdio(false);
cin.tie(0);
```

# ```.sort()``` 排序函式

+ ```.sort( 起始位置 , 結束位置 , 排序依據 0 or 1)```
+ 排序依據 預設為小到大

# 小數點輸出位數

```c
cout<<setprecision()<<....
```

#  ```setiosflags(ios::fixed)```
