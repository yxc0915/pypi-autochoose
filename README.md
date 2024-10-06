# PyPI 镜像源自动选择工具

## 项目简介

这个工具可以自动测试多个 PyPI 镜像源的速度，并为你选择最快的镜像源。它不仅可以显示测试结果，还能自动为你的 pip 配置最快的镜像源。

## 特性

- 自动测试多个知名 PyPI 镜像源的响应速度
- 智能选择最快的镜像源
- 自动配置 pip 使用最快的镜像源
- 支持结果缓存，避免频繁测试
- 多语言支持（目前支持中文和英文）
- 美观的命令行界面，使用 rich 库呈现结果

## 安装

1. 克隆此仓库：
   ```
   git clone https://github.com/your-username/pypi-mirror-selector.git
   cd pypi-mirror-selector
   ```

2. 运行脚本：
   ```
   python pypi_autochoose.py
   ```

   注意：脚本会自动安装所需的依赖（requests 和 rich）。

## 使用方法

直接运行脚本即可：

```
python pypi_autochoose.py
```

脚本将自动执行以下步骤：
1. 测试各个镜像源的速度
2. 显示测试结果
3. 选择最快的镜像源
4. 自动配置 pip 使用最快的镜像源

## 配置

你可以在 `lang_zh.py` 或 `lang_en.py` 文件中修改要测试的镜像源列表。

## 注意事项

- 请确保你有足够的权限来修改 pip 配置。
- 测试结果会缓存 1 小时，以减少不必要的网络请求。
- 如果遇到权限问题，可能需要以管理员身份运行脚本。

## 贡献

欢迎提交 Pull Requests 来改进这个项目。如果你有任何建议或发现了 bug，请开一个 issue。

## 许可证

本项目采用 MIT 许可证。详情请见 [LICENSE](LICENSE) 文件。
