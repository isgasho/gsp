# 14.2.6 並列forループ
forループ内を全てgoroutineで実行すれば並列化となる。ループ変数の実体はひとつしかないので、
goroutineの引数として渡し、groutineごとにコピーが作られるようにする必要がある。