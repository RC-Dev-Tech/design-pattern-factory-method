# ![](https://drive.google.com/uc?id=10INx5_pkhMcYRdx_OO4rXNXxcsvPtBYq) Factory Method Pattern 工廠方法模式 
> ##### 理論請自行找，網路上有很多相關的文章，這邊只關注於範例實作的部分.

---

<!--ts-->
## 目錄
* [目的](#目的)
* [使用時機](#使用時機)
* [URL結構圖](#url結構圖)
* [實作成員](#實作成員)
* [實作範例](#實作範例)
* [參考資料](#參考資料)
<!--te-->

---

## 目的
定義可生成物件的介面，但讓子類別去決定該具現出哪一種類別的物件.<br>
此模式讓類別將具現化程序交付給子類別去實作.

---

## 使用時機
* 當類別無法明確指定想要生成的物件類別時.
* 當類別希望讓子類別去指定想要生成的物件類型時.
* 當類別將權力下放給一個或多個輔助用途的子類別，但又希望將交付給子類別的實作集中在一處時.

---

## URL結構圖
![](https://drive.google.com/uc?id=1cKeKLErG4dnPn97iVP1t4krt6cnJ3mdT)
> 圖片來源：[Refactoring.Guru - Factory Method](https://refactoring.guru/design-patterns/factory-method)

---

## 實作成員
* Product
  * 定義Factory Method所造物件的介面
* ConcreteProduct
  * 具體實作出Product介面
* Creator
  * 宣告Factory Method，它會傳回Product型別之物件.<br>
    Factory Method預設的內容是傳回預設的ConcreteProduct物件.
* ConcreteCreator
  * 覆寫Factory Method以傳回ConcreteProduct的物件個體.

---

## 實作範例:
- [Example](https://github.com/RC-Dev-Tech/design-pattern-factory-method/blob/main/C%2B%2B/main.cpp) - Factory Method Pattern (C++)

---

## 參考資料
* [Wiki - Factory Method Pattern](https://en.wikipedia.org/wiki/Factory_method_pattern) <br>
* [Refactoring.Guru - Factory Method](https://refactoring.guru/design-patterns/factory-method) <br>

---

<!--ts-->
#### [目錄 ↩](#目錄)
<!--te-->
---
