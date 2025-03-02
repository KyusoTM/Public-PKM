# Javaの変数

## 変数名の慣習
- 1単語の変数名はすべて英子文字で記述する．
- 2単語以上の場合は[[camelCase]]で記述する
    - 記号・マルチバイト文字は使用しない．

## 特徴的な個所
1. データ型は先頭が大文字
   - `Byte`, `Long`等
2. long/floatは数値の末尾に接尾辞が必要．
```java
//それぞれ末尾に専用の英字が必要(大文字 or 小文字)
Float num = 173.4F;
Long num = 126500000L;
```
3. `final`修飾子
```java
   public class Main {
    public static void main(String... args) {
        final Integer money = 1000;
        System.out.println(money);
    }
}
```
4. 
