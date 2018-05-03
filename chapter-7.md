---
description: 'Names, Binding, Scope'
---

# Chapter 7

### 變數

命名

* 特殊字元
* 長度
* 大小寫
* special word
  * 保留字 reserved word
  * keyword

記憶體位置 Address

* l-value
* Struct 邊界對齊
  * \#pragma pack\(\[num\]\)
  * \#pragma pack\(\)
  * 變數大小
    * 整數
      * short -&gt; 2 bytes
      * int -&gt; 8 bytes
      * long -&gt; 8 bytes
    * 浮點數
      * float -&gt; 4 bytes
      * double -&gt; 8 bytes
      * long double -&gt; 12 bytes
    * 字元
      * char -&gt; 1 byte

Value

* R-value

Type

* range
* operation

### Binding

* Binding 的時機
  * 設計時
  * 執行時
  * 編譯時
  * Load time
  * Link time
  * Run time
* Static binding vs Dynamic Byding

Type Binding

* static type binding
  * explicit declaration
  * implicit declaration
* dynamic type binding



* Binding Lifetime
  * Allocation
  * Deallocation
  * classifier
    * static variable
    * stack
    * explicit heap
    * implicit heap
  * 

![](.gitbook/assets/image%20%281%29.png)

### scoping

* static scope
  * 巢狀結構
* dynamic scope
  * 方便
  * 變數可能被任何subprogram使用
  * impossible static type checking
  * 可讀性低
* block

-

* global scope
* referencing environment
* named constant

































