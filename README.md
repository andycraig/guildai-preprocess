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
result: 3.0
```

## Check results

```
guild compare
```
