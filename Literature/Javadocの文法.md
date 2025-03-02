# Javadocの文法

## 基本
文字列`/**`と`*/`の間にあるコメントが，ドキュメンテーションコメントとして`javadoc`に認識される．

ドキュメンテーションコメントは，以下の要素の**直前**に配置されている場合のみ認識され，それ以外の位置にあるコメントは無視される．
- クラス
- インターフェース
- コンストラクタ
- メソッド
- フィールド宣言

> [!WARNING]
> import文の前に挿入されたコメントは認識されない

### コメントの構造
ドキュメンテーションコメントは以下の2つのブロックに分けて認識される．

| ブロック         | 意味               | 範囲                         |
| ---------------- | ------------------ | ---------------------------- |
| 主説明           | コメント対象の概要 | `/**` から**最初のタグ**の間 |
| タグ・セクション | タグごとの説明     | **最初のタグ**から`*/`まで   |

javadocの例(Wikipedia)
```java
/**
 * Short one line description.                           (1)
 * <p>
 * Longer description. If there were any, it would be    (2)
 * here.
 * <p>
 * And even more explanations to follow in consecutive
 * paragraphs separated by HTML paragraph breaks.
 *
 * @param  variable Description text text text.          (3)
 * @return Description text text text.
 */
public int methodName (...) {
    // method body with a return statement
}
```

## タグの種類
| Tag & Parameter                  | Usage                                                                                                        | Applies to                              |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------- |
| @author John Smith               | 開発者名                                                                                                     | Class, Interface, Enum                  |
| {@docRoot}                       | ドキュメントのルートディレクトリからの相対パス                                                               | Class, Interface, Enum, Field, Method   |
| @version version                 | Provides software version information.                                                                       | Module, Package, Class, Interface, Enum |
| @since since-text                | 導入されたバージョン                                                                                         | Class, Interface, Enum, Field, Method   |
| @see reference                   | 関連する項目．                                                                                               | Class, Interface, Enum, Field, Method   |
| @param name description          | メソッドの引数に関する記述．引数の数だけ必要                                                                 | Method                                  |
| @return description              | Describes the return value.                                                                                  | Method                                  |
| @exception classname description | Describes an exception that may be thrown from this method.                                                  |                                         |
| @throws classname description    | Describes an exception that may be thrown from this method.                                                  | Method                                  |
| @deprecated description          | Describes an outdated method.                                                                                | Class, Interface, Enum, Field, Method   |
| {@inheritDoc}                    | Copies the description from the overridden method.                                                           | Overriding Method                       |
| {@link reference}                | Link to other symbol.                                                                                        | Class, Interface, Enum, Field, Method   |
| {@linkplain reference}           | Identical to {@link}, except the link's label is displayed in plain text than code font.                     | Class, Interface, Enum, Field, Method   |
| {@value ♯STATIC_FIELD}           | Return the value of a static field.                                                                          | Static Field                            |
| {@code literal}                  | Formats literal text in the code font. It is equivalent to <code>{@literal}</code>.                          | Class, Interface, Enum, Field, Method   |
| {@literal literal}               | Denotes literal text. The enclosed text is interpreted as not containing HTML markup or nested javadoc tags. | Class, Interface, Enum, Field, Method   |
| {@serial literal}                | Used in the doc comment for a default serializable field.                                                    | Field                                   |
| {@serialData literal}            | Documents the data written by the writeObject( ) or writeExternal( ) methods.                                | Field, Method                           |
| {@serialField literal}           | Documents an ObjectStreamField component.                                                                    | Field                                   |

## 参考
- Oracle: [javadoc](https://docs.oracle.com/javase/jp/8/docs/technotes/tools/windows/javadoc.html)
