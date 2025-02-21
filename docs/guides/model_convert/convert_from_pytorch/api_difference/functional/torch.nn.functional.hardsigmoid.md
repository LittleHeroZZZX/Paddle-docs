## [ paddle 参数更多 ]torch.nn.functional.hardsigmoid

### [torch.nn.functional.hardsigmoid](https://pytorch.org/docs/stable/generated/torch.nn.functional.hardsigmoid.html)

```python
torch.nn.functional.hardsigmoid(input, inplace=False)
```

### [paddle.nn.functional.hardsigmoid](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/nn/functional/hardsigmoid_cn.html#hardsigmoid)

```python
paddle.nn.functional.hardsigmoid(x, slope=0.1666667, offset=0.5, name=None)
```

其中 Paddle 相比 PyTorch 支持更多其他参数，具体如下：

### 参数映射

| PyTorch | PaddlePaddle | 备注 |
| ------- | ------------ | -- |
| input   | x            | 输入 Tensor，仅参数名不一致。 |
| -       | slope        | hardsigmoid 的斜率，PyTorch 无此参数，Paddle 保持默认即可。|
| -       | offset       | hardsigmoid 的截距，PyTorch 无此参数，Paddle 保持默认即可。|
| inplace | -            | 表示在不更改变量的内存地址的情况下，直接修改变量的值，Paddle 无此参数，一般对网络训练结果影响不大，可直接删除。 |
