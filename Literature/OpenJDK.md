# OpenJDK

[[Java SE]]及びその関連プロジェクトのオープンソース実装を行う「プロジェクト」または「リポジトリ」．

## 概要
[[Java SE]]ソースコードの開発プロジェクトであり，[公式サイト]または[Git]からアクセスするとソースコードを取得することができる．

ただし，サイトのソースコードはバイナリ化されていないため，そのままでは利用できない．

バイナリ化されたソースコードは[[Oracle]]もしくは，その他のグループがテスト・ビルドしたものを取得する必要がある．

## Open JDKの概念図
開発環境を構築するには，いずれかのグループがビルドしたバイナリコードをインストールする必要がある．

![alt text](<Private/Literature/Open JDKの概念図.png>)

## ビルドされたOpen JDKの一覧
Open JDKは6ヶ月に一度更新されるらしい．

Open JDK自体は[[OSS]]であり，無償で使用可能だが各企業によってサポート期間とその値段が異なる．

[[Oracle]]がビルドの有償化をしたことで，長期サポート[[LTS]]の費用を考慮する必要が出てきた．

| ビルド                         | ビルダー          | 商用サポート | LTS |
| ------------------------------ | ----------------- | ------------ | --- |
| [[Oracle Java SE]]             | [[Oracle]]        | 有償         | No  |
| [[Oracle OpenJDK]]             | [[Oracle]]        | 無償         | No  |
| [[AdoptOpenJDK]]               | [[Adoptium]]      | 無償         | 4y  |
| [[Zulu]]                       | [[Azule Systems]] |              | 8y  |
| [[Microsoft Build of OpenJDK]] | Microsoft         | 有償         |     |
| [[Amazon Corretto]]            | [[Amazon]]        | 無償         |     |


## 参考
- Orakle JDK : [公式サイト]，[Git]
- Qiita : [JDK、Oracle JDK、OpenJDK、Java SEってなに？](https://qiita.com/nowokay/items/c1de127354cd1b0ddc5e)
- Qiita : [JDKの長期商用サポート(LTS)の提供ベンダー比較（無償利用についても言及あり）](https://qiita.com/u-tanick/items/bb166929a58a4c20bb88)

[公式サイト]: https://openjdk.org/
[Git]: https://github.com/openjdk/jdk

[//begin]: # "Autogenerated link references for markdown compatibility"
[Java SE]: <Java SE.md> "Java SE"
[//end]: # "Autogenerated link references"