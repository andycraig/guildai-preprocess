# Guild AI preprocessing example

## Preprocess

```
guild run example:prepare alpha=2
```

## Train

```
guild runs -o prepare
```

Copy ID of run

```
guild run example:train preprocessed=[ID you copied]
```

Should output:

```
result: 3
```

## Check results

```
guild compare
```

Output should be like:

```
run       operation        started              time     status     label    step  result  alpha
d7a79517  example:train    2020-03-07 18:42:33  0:00:00  completed           0     3.0
1acdd79d  example:prepare  2020-03-07 18:42:03  0:00:00  completed  alpha=2                2
```

