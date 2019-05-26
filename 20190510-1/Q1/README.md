# Q1 走出自己的風格

## 題目敘述

恭喜你進入了世界上最簡單的迷宮，這個迷宮是一個 N * N 的方陣，你需要從迷宮的最左上角開始走到方陣的最右下角。此時你發現地上有前人走向出口的足跡，但一件這麼簡單的事情你認為你不想走跟前人一樣的路，甚至你會特別去避開走任何跟前人一樣的路。如下圖：

![](https://i.imgur.com/m3oMKpw.png)
> 藍色為前人的走法，橘色為其中一種你認為能行的走法

如果前人的走法中包含「 A 格走向 C 格」，則你會避開不從「 A 格走向 C 格」，但「從 B 格走向 C 格」是你可以接受的。

## 輸入
輸入的第一行 T 為測試筆數。
每個測試筆數有兩行組成：第一行為整數 N，表示迷宮的長跟寬。
第二行為長度 2N-2 的字串，由 `S` 跟 `E` 兩種字母組成， `S` 代表往南走、`E` 代表往東走。代表為前人走過的走法。

## 輸出
針對每筆測試輸出 `Case #x: y` ，其中 x 是該筆測試的編號。
y 為長度 2N - 2 的字串，由 `S` 跟 `E` 兩種字母組成， `S` 代表往南走、`E` 代表往東走。
輸出一種滿足上敘原則的路徑

## 測資範圍

1 ≤ T ≤ 100.
前人的足跡一定可以走向終點
小測資集 : 2 ≤ N ≤ 10. Time limit (15 seconds)
大測資集 : 2 ≤ N ≤ 1000. Time limit (15 seconds)
超大測資集 : 2 ≤ N ≤ 50000. Time limit (15 seconds)

## 範例
輸入
```
3
3
EESS
4
ESESES
5
ESSESESE
```

輸出
```
Case #1: SSEE
Case #2: SSESEE
Case #3: SEEESSES
```

* 針對 Case #1 輸出 SESE 的話也是正解
* 針對 Case #3 如同上方圖中所示。