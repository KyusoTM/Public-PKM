# SQL文

[[SQL]]を用いて，[[DB]]に対して問い合わせができる形式に処理がまとめられた文．

```sql
-- sakilaデータベースを用いた例(MySQL)
-- 名前を降順にして10名文のテーブルを取得
SELECT * FROM sakila.actor
ORDER BY first_name DESC
LIMIT 10;
```

[//begin]: # "Autogenerated link references for markdown compatibility"
[SQL]: SQL.md "SQL"
[//end]: # "Autogenerated link references"