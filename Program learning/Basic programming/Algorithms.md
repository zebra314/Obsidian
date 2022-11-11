---
tags: programming, competitive_programming, c++ 
---
# LIS基礎演算法

1. 時間複雜度:O(n<sup>2</sup>)
2. Code:

```c
#include<bits/stdc++.h>
using namespace std;
int main()
{
    int i, j, k;
    vector<pair<int, int>> a;
    map<int, int> b;
    while (cin >> k)
    {
        a.push_back(make_pair(k, 1));
        for (i = 0; i < a.size(); i++)
        {
            for (j = 0; j <= i; j++)
            {
                if (a[i] > a[j])
                {
                    a[i].second = max(a[i].second, a[j].second + 1);
                }
            }
            b[a[i].second] = a[i].first;
        }
    }
    cout << b.size() << "\n"
         << "-"
         << "\n";
    for (auto l : b)
    {
        cout << l.second << "\n";
    }
}
```

# LIS進階演算法(只求長度)

1. 時間複雜度:O(n_log_n)
2. DP, Greedy, Binary search
3. Code:

```c
#include<bits/stdc++.h>
using namespace std;
int main()
{
    int a,d,i;
    vector<long int>b,c;
    while(cin>>a){b.push_back(a);}
    for(i=1;i<b.size();i++)
    {
        if(c.empty() or b[i]>c.back())  c.push_back(b[i]);      //置入
        else {  *lower_bound(c.begin(),c.end(),b[i])=b[i];    } //取代
    }
    cout<<c.size()<<"\n"<<"-"<<"\n";
}
```

# Binary Search

```c
int binary_search(vector<int>v,int target) //find the position 
{
    int left=0;
    int right=v.size()-1;
    while(right=>left)
    {
        int mid=(right+left)/2;
        if(target==v[mid])  return left; //最後的解 left下界 right上界
        if(target>v[mid])   left=mid+1;
        else    // target<v[mid] 
            right=mid-1;
    }
    return -1;//fail
}
```

# 輾轉相除法

1. 求最大公因數

```c
    while(b!=0 and c!=0)
    {
        if(b>=c)
            b=b%c;
        else
            c=c%b;
    }
    //最大公因數為max(b,c)
```

# types of algorithms
1. 排序 搜尋法
2. greedy 
3. dynamic programming
4. graph traversal
	1. tree cut
5. minimum spanning tree
	1. prim 
	2. kruskal 
6. Shortest Path
	1. Bellman-Ford
	2. Dijkstra
	3. Floyd-Warshall
	4. A*
7. maximum flow (hard)