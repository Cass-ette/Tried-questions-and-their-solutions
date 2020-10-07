[数列递推](https://loj.ac/problem/538)

【题解】容易发现数列最后一定单调，最后单调递增则最大值赋为最后一个，反之最小值赋为最后一个，然后处理一些细节就可以AC，要注意以下几点：

1.数列连续三项以及数列最后一项>10^7时退出。

2.可能第一要求项就比你枚举的大，需要特判。

3.要求项的枚举不能等于最大项，不然会无法正常指向最后一个。

这其实是一道纯真·暴力啊？

很简单的试着写暴力以后就能发现，到一定程度以后数列就会呈现出单调的趋势

更准确的说，当连续两个数的符号相同以后，数列就一定单调了

官网题解上有严格证明说，这样的情况，数列项数不会超过36项

[](https://images2017.cnblogs.com/blog/1138649/201711/1138649-20171108175311684-293574685.jpg)

这样的话，直接暴力前几项，然后对集合排个序就可以高辣......

感觉我的常数写的还是不错的.....
