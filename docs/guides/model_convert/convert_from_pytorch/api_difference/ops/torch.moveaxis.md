## [ 仅参数名不一致 ]torch.moveaxis
### [torch.moveaxis](https://pytorch.org/docs/stable/generated/torch.moveaxis.html?highlight=moveaxis#torch.moveaxis)

```python
torch.moveaxis(input,
               source,
               destination)
```

### [paddle.moveaxis](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/moveaxis_cn.html#moveaxis)

```python
paddle.moveaxis(x,
                source,
                destination,
                name=None)
```

两者功能一致且参数用法一致，仅参数名不一致，具体如下：
### 参数映射
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| <font color='red'> input </font> | <font color='red'> x </font> | 表示输入的 Tensor ，仅参数名不一致。  |
| <font color='red'> source </font> | <font color='red'> source </font> | 表示将被移动的轴的位置，仅参数名不一致。  |
| <font color='red'> destination </font> | <font color='red'> destination </font> | 表示轴被移动后的目标位置，仅参数名不一致。  |
