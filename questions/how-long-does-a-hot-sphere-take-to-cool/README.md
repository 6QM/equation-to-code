# 01 · 热金属球多久冷却到目标温度？

打开 [experiment.ipynb](experiment.ipynb)，从顶部依次运行。先看结果、改参数，再回头理解能量守恒与数值方法。

假设半径 1 cm 的均匀金属球从 80 °C 冷却到 40 °C，周围流体保持 20 °C。忽略辐射、支撑导热与物性变化，指定 h = 25 W/(m² K)。这是原创教学模型，不是教材原题或实验结果。

默认结果：集总模型预测约 **356 秒（5.93 分钟）**，Bi ≈ 0.000407。Notebook 包含解析曲线、Euler 近似、步长误差比较，以及模型适用性与结果检查。

## 运行

在仓库根目录，使用 Python 3.9 或以上（建议 3.11）：

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyterlab
```

Windows 激活方式：`.venv\Scripts\activate`。选择该环境的 Python kernel，再执行 Restart Kernel and Run All。

命令行验证：

```bash
python -m jupyter nbconvert --to notebook --execute --inplace questions/how-long-does-a-hot-sphere-take-to-cool/experiment.ipynb
```

首轮只需完成三个任务：跑通、把 h 改为 50 并重新运行、用自己的话解释曲线为何变化。未理解的数学先标注，后面的拆解部分会逐项解释。

教材对应主题见 [引用说明](../../references/core-textbooks.md)，后续问题见 [学习路线](../../maps/heat-transfer-learning-path.md)。
