RMeCabパッケージとは
========================================================
RMeCabは日本語形態素解析である MeCab とRを接続するインターフェイスです．RMeCabは以下からダウンロードすることができます．

http://rmecab.jp/wiki/index.php?RMeCab

RMeCabを試す
-------------------------



```r
# RMeCab を利用する準備
library(RMeCab)
```




### 文字を単位としたNgram(bigram)を生成


```r
# 鴎外と漱石それぞれ4作品を含むフォルダを指定
res <- docNgram ("D:/fromC/data/writers", type = 0) # writers はフォルダ名
```

```
## Error: no doc-matrix returned.
```

```r

res2 <- res[ rownames(res) %in% c("[と-、]", "[て-、]", 
                                  "[は-、]", "[が-、]", 
                                  "[で-、]",  "[に-、]",  
                                  "[ら-、]",  "[も-、]" ) 
```

```
## Error: オブジェクト 'res' がありません
```

```r
res2
```

```
## Error: オブジェクト 'res2' がありません
```

```r
res2.pc <- princomp (t (res2))
```

```
## Error: オブジェクト 'res2' がありません
```




### 主成分分析によるバイプロット



```r
biplot(res2.pc)
```

```
## Error: オブジェクト 'res2.pc' がありません
```



このプロジェクトは以下に公開しています
