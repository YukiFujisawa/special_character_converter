## 概要
特殊文字をescapeするツールです。

|文字|escape|
|---|---|
|改行|\n|
|タブ|\t|
|ダブルクオート|\"|
|シングルクオート|\'|

## サンプル

### 変換前

```python
rowNum = int(input())

for i in range(rowNum):
    inputs = input()
    if inputs == "[]":
        inputs = []
    else: // テスト
        inputs = inputs.rstrip().split(' ')
        inputs = list(map(float, inputs))

    print(check_sample(inputs))
```

### 変換後


```python
rowNum = int(input())\n\nfor i in range(rowNum):\n    inputs = input()\n    if inputs == \"[]\":\n        inputs = []\n    else: // テスト\n        inputs = inputs.rstrip().split(\' \')\n        inputs = list(map(float, inputs))\n\n    print(check_sample(inputs))
```