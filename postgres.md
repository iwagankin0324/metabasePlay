```sh
cd app/build/
docker compose up -d
docker exec -i -t postgres16 bash
psql -U postgres -d postgres
```

```sql
\d
select * from access_log;
quit
```

データ投入
https://zenn.dev/sikkim/articles/6866b32919372d

データベース操作
https://qiita.com/Utsubo/items/04aa2281046cf55aee1a
