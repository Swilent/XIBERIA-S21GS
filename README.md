# 西伯利亚S21GS 频响数据与EQ调音

这个项目包含了西伯利亚S21GS耳机的频响数据和均衡器(EQ)调音文件，帮助用户获得更好的音频体验。

## 📁 项目文件

| 文件名 | 描述 |
|--------|------|
| [`西伯利亚S21GS.csv`](./西伯利亚S21GS.csv) | 原始频响数据 |
| [`西伯利亚S21GS GraphicEq.txt`](./西伯利亚S21GS GraphicEq.txt) | EqualizerAPO GraphicEQ格式文件 |
| [`西伯利亚S21GS ParametricEq.txt`](./西伯利亚S21GS ParametricEq.txt) | EqualizerAPO ParametricEq格式文件 |

## 📊 频响数据来源

- **数据来源**: [西伯利亚 S21GS火焰风暴频响曲线](https://huihifi.com/evaluation/cb4e87ff-fa4a-4825-b5a8-250541386c13)
- **数据版权**: 毁HiFi|专业耳机数据测评网站所有
- **说明**: 西伯利亚 S21GS火焰风暴为西伯利亚S21GS的特殊涂装版本，发声单元没有区别，频响数据相同

## 🔧 EQ调音说明

### 生成过程
1. 使用 [AutoEQ](https://autoeq.app/) 平台（[GitHub仓库](https://github.com/jaakkopasanen/AutoEq)）
2. 导入 `西伯利亚S21GS.csv` 文件
3. 设置目标频响曲线为 **Harman over-ear 2018**
4. 生成两种格式的EQ文件：
   - EqualizerAPO GraphicEQ 格式
   - EqualizerAPO ParametricEq 格式

### Windows平台使用指南 (推荐)

本人在Windows平台使用 **Equalizer APO** 进行EQ调音：

#### 安装步骤
1. 下载并安装 [Equalizer APO](https://sourceforge.net/projects/equalizerapo/)
2. 将 [`西伯利亚S21GS GraphicEq.txt`](./西伯利亚S21GS GraphicEq.txt) 文件复制到Equalizer APO安装目录下的 `config` 文件夹
3. 编辑 `config` 文件夹中的配置文件，添加以下内容：

```ini
Include: 西伯利亚S21GS GraphicEq.txt  ; 使用这个eq文件
Device: 扬声器 S21GS                  ; 仅在使用S21GS时启用
```

## 🎧 其他平台使用

对于其他平台或均衡器软件，您可以：

1. 访问 [AutoEQ](https://autoeq.app/)
2. 导入本项目的 [`西伯利亚S21GS.csv`](./西伯利亚S21GS.csv) 文件
3. 根据您的需求选择：
   - 目标频响曲线（如Harman over-ear 2018、diffuse field等）
   - 支持的均衡器软件格式
   - 适合您设备的EQ参数

## 📄 许可证

本项目采用 [CC BY-SA 4.0](./LICENSE)（知识共享署名-相同方式共享 4.0 国际许可协议）许可证。

## ⚠️ 免责声明

- 频响数据来源于毁HiFi|专业耳机数据测评网站，版权归原网站所有
- EQ文件仅供参考，实际效果可能因设备差异和个人偏好而不同
- 使用EQ前请备份原始设置，谨慎调整音量以避免听力损伤

---
