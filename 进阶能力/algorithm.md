排序算法
===========

最快最简单的排序--桶排序
----------------------

适用范围：正整数排序

算法复杂度：M+N （M:桶的个数 N:数组的长度）

测试数据：[5,3,5,2,8]

C语言版本

```C

    #include <stdio.h>
    int main(){
        int a[11],i,j,t,n;
        // 初始化11个桶 m
        for(i=0;i<=10,i++){
            a[i] = 0
        }
        scanf("%d",&t);
        // 循环读入n个数 n
        for(i=0;i<=n;i++){
            scanf("%d",&t);
            a[t]++;
        }
        // 排序 m+n
        for(i=0;i<=10;i++){
            for(j=0;j<=a[i];j++){
              printf("%d",i);
            }  
        }
        return 0;
    }
```

Javascript 版本

```javascript

    function sort(arr){
        // 申请桶 m
        const a = new Array(10);
        a.fill(0);

        //  循环读入 n
        for(let i=0,len=arr.length;i<len;i++){
            const value = arr[i];
            a[value]++
        }

        // 排序 m+n
        for(let i=0,len=a.length;i<len;i++){
            for(let j=0;j<a[i];j++){
                console.log(i);
            }
        }

    }

```