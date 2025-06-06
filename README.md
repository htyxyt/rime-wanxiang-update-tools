# Rime 万象更新工具

## 项目简介

本工具用于自动更新Rime输入法的万象方案、词库和模型，支持Windows、macOS和Linux系统。

## 工具版本计划

- [x] [Windows版本](./Windows/README.md)
- [x] [macOS版本](./Mac/README.md)
- [x] [Linux版本](./Linux/README.md)

### Windows版本

- **版本区别**
  - **执行环境**: PowerShell 运行环境 Windows 10 自带，Python 需要自己安装 Python 环境
  - **运行方式**: PowerShell版本直接双击运行；Python版本需要命令行执行
  - **功能实现**: 两个版本功能相同，但Python版本更易于跨平台移植
    - Python 版本支持 GitHub 镜像加速

- [x] [PowerShell版本](./Windows/PowerShell/README.md)
  - 下载链接：[按需下载万象方案-词库-模型(GBK版本：文件名：**rime-wanxiang-update-windows.ps1**)](https://github.com/expoli/rime-wanxiang-update-tools/releases/latest/download/rime-wanxiang-update-windows.ps1)
  - 下载链接：[按需下载万象方案-词库-模型(UTF-8版本：文件名：**rime-wanxiang-update-windows-utf-8.ps1**](https://github.com/expoli/rime-wanxiang-update-tools/releases/latest/download/rime-wanxiang-update-windows-utf-8.ps1)
- [x] [Python版本](./Windows/Python/README.md)
  - 下载链接：[Windows/Python/按需下载万象方案-词库-模型.py](https://github.com/expoli/rime-wanxiang-update-tools/raw/refs/heads/main/Windows/Python/%E6%8C%89%E9%9C%80%E4%B8%8B%E8%BD%BD%E4%B8%87%E8%B1%A1%E6%96%B9%E6%A1%88-%E8%AF%8D%E5%BA%93-%E6%A8%A1%E5%9E%8B.py)
  - 下载链接：[rime-wanxiang-update-windows.py](https://github.com/expoli/rime-wanxiang-update-tools/releases/latest/download/rime-wanxiang-update-windows.py)

### macOS版本
- [x] [Python版本](./Mac/Python/README.md)


### Linux版本

- [x] [Shell版本](./Linux/Shell/README.md)
  - 下载链接：[Linux/Shell/wanxiang-update](https://github.com/expoli/rime-wanxiang-update-tools/releases/latest/download/linux-wanxiang-update)

## 使用说明

1. 选择对应的系统版本
2. 按照说明文档进行操作
3. 工具将自动完成更新
4. Windows 默认不支持无签名的 ps 脚本运行，如果右键运行失败，请在终端中运行，如果提示如下错误：

```PowerShell
C:\Users\12418\Desktop\按需下载万象方案-词库-模型.ps1，因为在此系统上禁止运行脚本。有关详细信息，请参阅 https:/go.microsoft.com/fwlink/?LinkID=135170 中的 about_Executio
n_Policies。
所在位置 行:1 字符: 1
+ C:\Users\12418\Desktop\按需下载万象方案-词库-模型.ps1
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : SecurityError: (:) []，PSSecurityException
    + FullyQualifiedErrorId : UnauthorizedAccess
```

请在终端中运行以下命令，然后再运行脚本即可。 

```PowerShell
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser
```

## 许可证

MIT License
