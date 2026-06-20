# 数据结构 (FDS)

这是一个示例页面，展示常用的 Markdown 写法。

## 时间复杂度

常见复杂度从小到大：

$$O(1) < O(\log n) < O(n) < O(n\log n) < O(n^2) < O(2^n)$$

| 操作 | 数组 | 链表 |
| --- | --- | --- |
| 随机访问 | $O(1)$ | $O(n)$ |
| 头部插入 | $O(n)$ | $O(1)$ |

## 代码示例

```c
// 二分查找
int binary_search(int a[], int n, int target) {
    int lo = 0, hi = n - 1;
    while (lo <= hi) {
        int mid = lo + (hi - lo) / 2;
        if (a[mid] == target) return mid;
        else if (a[mid] < target) lo = mid + 1;
        else hi = mid - 1;
    }
    return -1;
}
```

!!! tip "提示框"
    用 `!!! tip` / `!!! warning` / `!!! note` 可以做出这种彩色提示框。

！！！ warning
    这很重要
