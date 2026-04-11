# ostep-code
下面这段话是我询问mimo现在ai如此强大，是否还有必要学习分页这样的原理得到的答案

> 这就像学物理的人觉得牛顿力学用不上——你不会每天算力的分解，但它会变成你理解世界的直觉。分页原理也是一样，它不会出现在你每天的代码里，但它会在你排查性能问题、理解系统行为的时候，给你一个别人没有的视角。
真正"用不上"的时刻，往往是你还没碰到足够难的问题。

## 仓库介绍

本仓库是《操作系统导论》(Operating Systems: Three Easy Pieces) 一书的配套学习资源，主要包含：

- 课后习题的代码实现(非标准答案)
- 章节笔记总结
- 针对Python 3的代码兼容性修改

英文原版教材：http://pages.cs.wisc.edu/~remzi/OSTEP/
README部分参考翻译：https://github.com/joshuap233/Operating-Systems-Three-Easy-Pieces-NOTES/tree/main

## 目录结构

仓库采用章节编号+章节名称的目录结构，便于按章节查找和学习：

```
├── 04.抽象:进程/          # 第4章：进程抽象
│   ├── process-run.py     # 进程运行模拟代码
│   ├── 总结.md           # 章节学习笔记
│   └── README-process-run-翻译.md  # 代码使用说明（翻译版）
└── README.md              # 仓库说明文档
```

## 环境要求

- 操作系统：Linux (推荐Fedora 43+) 或其他类Unix系统
- 编译器：GCC 15.2.1+ (用于C语言代码)
- Python版本：Python 3.10+ (已将原Python 2代码迁移到Python 3)

## 使用方法

### 1. 克隆仓库

```bash
git clone https://github.com/your-username/ostep-code.git
cd ostep-code
```

### 2. 运行代码

进入对应章节目录，运行相应的代码文件：

```bash
# 以第4章进程模拟代码为例
cd 04.抽象:进程
python3 process-run.py -h
```

### 3. 查看学习资源

- 每个章节目录下的`总结.md`包含章节重点内容和学习笔记
- 部分代码文件配有详细的使用说明文档

## 代码迁移说明

原教材配套代码基于Python 2编写，本仓库已将其迁移到Python 3，主要修改包括：

- 更新print语句为print()函数
- 修复exit()函数调用
- 确保字符串处理的兼容性
- 保持原有功能和行为不变

## 贡献指南

欢迎提交：
- 代码优化建议
- 习题答案补充
- 学习笔记分享
- 其他改进建议

## 许可证

遵循原教材代码的许可证协议。

## 致谢

感谢Remzi H. Arpaci-Dusseau和Andrea C. Arpaci-Dusseau教授编写的优秀教材！