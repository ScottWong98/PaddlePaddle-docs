## [参数不一致]torch.nn.functional.gelu

### [torch.nn.functional.gelu](https://pytorch.org/docs/stable/generated/torch.nn.functional.gelu.html#torch.nn.functional.gelu)

```python
torch.nn.functional.gelu(input, approximate='none')
```

### [paddle.nn.functional.gelu](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/nn/functional/gelu_cn.html)

```python
paddle.nn.functional.gelu(x, approximate=False, name=None)
```

其中功能一致, 输入参数用法不一致，具体如下：

### 参数映射

| PyTorch     | PaddlePaddle | 备注                                                                                 |
| ----------- | ------------ | ------------------------------------------------------------------------------------ |
| input       | x            | 输入的 Tensor，仅参数名不一致。                                                      |
| approximate | approximate  | 是否使用近似计算，PyTorch 取值 none 和 tanh，Paddle 取值为 bool 类型，需要转写。 |

### 转写示例

#### approximate 参数：是否使用近似计算

```python
# PyTorch 写法:
y1 = torch.nn.functional.gelu(x, approximate='tanh')
y2 = torch.nn.functional.gelu(x, approximate='none')

# Paddle 写法:
y1 = paddle.nn.functional.gelu(x, approximate=True)
y2 = paddle.nn.functional.gelu(x, approximate=False)
```
