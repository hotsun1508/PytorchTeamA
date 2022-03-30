# PytorchTeamA


# 파이토치 풀잎

CNN 파이토치 프로젝트

구글 드라이브에 넣어서 zip 풀고 colab 에서 진행하시면 됩니다.

[02_cnn_pt.zip](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0411a930-b0d3-4aa3-8ab5-9c8e59549978/02_cnn_pt.zip)

추가적으로 zip 파일 풀어보시면 [checker.py](http://checker.py) 라는 파일이 있는데  이 파일에 오류가 있어서 수정해줘야합니다.  

65번 째줄에

```python
print(f'{dataset.mode}의 **len** 함수가 train_data의 데이터 갯수를 2000이 아닌 {}으로 반환하고 있습니다. 가지고 있는 데이터셋 또는 __len__함수 구현에 문제가 없는지 다시 확인하시기 바랍니다.'.format(len(dataset)))
```

를

```python
print(f'{dataset.mode}의 **len** 함수가 train_data의 데이터 갯수를 2000이 아닌 {len(dataset)}으로 반환하고 있습니다. 가지고 있는 데이터셋 또는 __len__함수 구현에 문제가 없는지 다시 확인하시기 바랍니다.')
```

으로 바꿔야합니다
