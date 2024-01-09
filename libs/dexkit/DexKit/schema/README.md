# DexKit FlatBuffer schema

## python generate kotlin && c++ code

```shell
python gen_code.py
```

## kotlin

```shell
./flatc --kotlin -o ../dexkit/src/main/java/org/luckypray \
fbs/encode_value.fbs fbs/enums.fbs fbs/matchers.fbs fbs/querys.fbs fbs/ranges.fbs fbs/results.fbs
```

## c++

```shell
./flatc -c --cpp-std c++17 --scoped-enums --no-emit-min-max-enum-values -o ../Core/dexkit/include/schema \
fbs/encode_value.fbs fbs/enums.fbs fbs/matchers.fbs fbs/querys.fbs fbs/ranges.fbs fbs/results.fbs
```
