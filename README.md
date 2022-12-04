# Multi-LD

结合CA-MKD进行多教师蒸馏的LD改进版本，使用了Wasserstein Loss来计算CA-MKD的权重。

## 训练

在训练前，你需要配置与LD相同的环境（参见 [INSTALL.md](docs/install.md)）并将COCO数据集放置在`data/coco/`.

运行以下命令以在COCO训练集上训练。

```
./tools/dist_train.sh configs/multi_ld/multi_ld_r18_fpn_coco_1x.py 8
```

**注意：**在开始训练前，你很可能需要调整该config文件（`configs/multi_ld/multi_ld_r18_fpn_coco_1x.py`）以适应你的机器设置。
