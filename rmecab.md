RMeCab�p�b�P�[�W�Ƃ�
========================================================
RMeCab�͓��{��`�ԑf��͂ł��� MeCab ��R��ڑ�����C���^�[�t�F�C�X�ł��DRMeCab�͈ȉ�����_�E�����[�h���邱�Ƃ��ł��܂��D

http://rmecab.jp/wiki/index.php?RMeCab

RMeCab������
-------------------------



```r
# RMeCab �𗘗p���鏀��
library(RMeCab)
```




### ������P�ʂƂ���Ngram(bigram)�𐶐�


```r
# ���O�Ɵ��΂��ꂼ��4��i���܂ރt�H���_���w��
res <- docNgram ("D:/fromC/data/writers", type = 0) # writers �̓t�H���_��
```

```
## Error: no doc-matrix returned.
```

```r

res2 <- res[ rownames(res) %in% c("[��-�A]", "[��-�A]", 
                                  "[��-�A]", "[��-�A]", 
                                  "[��-�A]",  "[��-�A]",  
                                  "[��-�A]",  "[��-�A]" ) 
```

```
## Error: �I�u�W�F�N�g 'res' ������܂���
```

```r
res2
```

```
## Error: �I�u�W�F�N�g 'res2' ������܂���
```

```r
res2.pc <- princomp (t (res2))
```

```
## Error: �I�u�W�F�N�g 'res2' ������܂���
```




### �听�����͂ɂ��o�C�v���b�g



```r
biplot(res2.pc)
```

```
## Error: �I�u�W�F�N�g 'res2.pc' ������܂���
```



���̃v���W�F�N�g�͈ȉ��Ɍ��J���Ă��܂�
