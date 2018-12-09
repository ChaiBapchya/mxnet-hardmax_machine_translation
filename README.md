# mxnet-hardmax_machine_translation
Using Hardmax operator in Apache MXNet framework for performing Machine Translation

# Data

## Retrieving data

```
wget http://www.statmt.org/europarl/v7/fr-en.tgz
```
```
tar -xzvf fr-en.tgz
```

## Downsizing
Originally the files were 288MB long with 2007723 lines
```
du -h europarl-v7.fr-en.fr
288M	europarl-v7.fr-en.fr
```
```
$ wc -l europarl-v7.fr-en.fr
2007723 europarl-v7.fr-en.fr
```

For demonstration purpose, we shorten them.

```
head -100000 europarl-v7.fr-en.fr > tiny.europarl-v7.fr-en.fr
```

Result
tiny.europarl-v7.fr-en.fr and tiny.europarl-v7.fr-en.en
100000 lines and 16MB
