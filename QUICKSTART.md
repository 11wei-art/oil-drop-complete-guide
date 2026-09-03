# ⚡ 快速开始指南（5分钟上手）

## 🎯 目标
在 5 分钟内下载完整的油滴检测数据集。

## 📋 前置要求

- ✅ 电脑上安装了 Python 3.7 以上
- ✅ 磁盘有 2GB+ 可用空间
- ✅ 网络连接正常

**检查 Python 版本：**
```bash
python --version
```

如果显示版本号，说明已安装。如果没有，请先 [安装 Python](https://www.python.org/downloads/)

---

## 🚀 5 分钟快速上手

### 第 1 步：下载项目（1 分钟）

**方法 A：用 Git 克隆（如果装了 Git）**
```bash
git clone https://github.com/11wei-art/oil-drop-complete-guide.git
cd oil-drop-complete-guide
```

**方法 B：手动下载 ZIP**
1. 点击这个链接：[Download ZIP](https://github.com/11wei-art/oil-drop-complete-guide/archive/refs/heads/main.zip)
2. 解压到你的电脑
3. 打开解压后的文件夹

### 第 2 步：安装依赖（1 分钟）

打开**命令提示符**（Windows）或**终端**（Mac/Linux），进入项目文件夹，运行：

```bash
pip install -r requirements.txt
```

会安装 3 个库：requests、tqdm、pyyaml

### 第 3 步：运行下载脚本（3 分钟）

```bash
python download_datasets.py
```

你会看到菜单：
```
主菜单:
1. 一键下载所有数据集 (推荐)
2. 查看数据集信息
3. 自定义下载单个数据集
4. 查看已下载数据
5. 退出

请选择 (1-5): 
```

**输入 `1` 然后按 Enter**

### 第 4 步：等待下载

脚本会自动下载所有 4 个数据集，显示进度条：

```
[==================================================] 100%
✓ 下载完成！
```

根据网络速度，需要 **30分钟 - 2小时**。

---

## 📂 数据在哪里？

下载完成后，你会看到这个文件夹结构：

```
油滴检测项目/
├── download_datasets.py     (下载脚本)
├── check_data.py            (数据检查脚本)
├── README.md                (详细文档)
├── QUICKSTART.md            (这个文件)
└── data/                    ← 数据在这里！
    ├── dataset_1_iSort/             (103 MB)
    ├── dataset_2_microscopy/        (948 MB) ⭐
    ├── dataset_3_dmv_tool/          (0.2 MB)
    └── dataset_4_python_scripts/    (0.1 MB)
```

打开 `data/` 文件夹就能看到所有下载的数据！

---

## ✅ 检查下载结果

下载完成后，运行这个命令查看统计信息：

```bash
python check_data.py
```

会显示：
```
📊 数据统计信息
=================================================================

📁 已下载的数据集:

📁 dataset_1_iSort_-_自动化液滴分类数据
   📄 文件数: 25
   💾 大小: 103.48 MB

📁 dataset_2_液滴显微镜图像和荧光光谱数据
   📄 文件数: 220
   💾 大小: 947.98 MB

... (更多统计)

📊 汇总统计:
   数据集数量: 4
   文件总数: 246
   总大小: 1.05 GB
   保存位置: C:\...\data\
```

---

## ❓ 常见问题

### Q1: 下载失败了怎么办？

**A:** 这通常是网络问题，解决方案：
1. 检查网络连接
2. 重新运行脚本（会继续下载）
3. 等几分钟后再试

### Q2: 显示 "找不到 git"

**A:** 这不是问题！你是手动下载的 ZIP，不需要 Git。

### Q3: 显示 "ModuleNotFoundError"

**A:** 说明依赖没装好。运行：
```bash
pip install -r requirements.txt --upgrade
```

### Q4: 下载非常慢

**A:** 
- 检查网络速度
- 关闭其他下载和视频播放
- 稍后重新尝试

### Q5: 需要多大空间？

**A:** 至少 2GB（建议 5GB）。可以运行：
```bash
# Windows
dir C:\

# Mac/Linux
df -h
```

查看可用空间。

---

## 🎓 下载完后可以做什么？

### 1. 查看详细文档
```bash
cat README.md
```

### 2. 查看数据内容
打开 `data/` 文件夹，浏览图像和数据

### 3. 开始训练模型
用这些数据训练 YOLO、Mask R-CNN 等深度学习模型

### 4. 标注更多数据
使用标注工具标注新图像

---

## 📞 需要帮助？

遇到问题，可以：

1. 查看本文档的 [常见问题](#常见问题) 部分
2. 查看详细的 [README.md](README.md)
3. 在 GitHub 提交 Issue

---

## 🎉 恭喜！

现在你已经掌握了如何下载油滴检测数据集！

**下一步？** 打开 [README.md](README.md) 学习如何使用这些数据。

---

**预计时间：** 30分钟 - 2小时  
**需要空间：** 2 GB  
**难度：** ⭐ 非常简单

祝你成功！ 🌟
