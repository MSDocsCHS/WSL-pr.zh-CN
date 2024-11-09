---
title: 什么是适用于 Linux 的 Windows 子系统
description: Learn about the Windows Subsystem for Linux, including the different versions and ways you can use them. Microsoft Loves Linux.
ms.date: 11/20/2023
ms.topic: article
---

# 什么是适用于 Linux 的 Windows 子系统？

适用于 Linux 的 Windows 子系统 (WSL) 是 Windows 的一个功能，允许您在 Windows 机器上运行 Linux 环境，而无需单独的虚拟机或双系统。WSL 旨在为希望同时使用 Windows 和 Linux 的开发人员提供无缝且高效的体验。

- 使用 WSL 安装和运行各种 Linux 发行版，如 Ubuntu、Debian、Kali 等。[安装 Linux 发行版](./install.md) 并从 [Microsoft Store](./compare-versions.md#wsl-in-the-microsoft-store) 接收自动更新，或 [导入不在 Microsoft Store 中可用的 Linux 发行版](./use-custom-distro.md)，或 [构建自己的自定义 Linux 发行版](./build-custom-distro.md)。
- 在已安装的发行版中的隔离的 Linux 文件系统中存储文件。
- 运行命令行工具，如 BASH。
- 运行常见的 BASH 命令行工具，如 `grep`、`sed`、`awk` 或其他 ELF-64 二进制文件。
- 运行 Bash 脚本和 GNU/Linux 命令行应用程序，包括：  
  - 工具：vim、emacs、tmux
  - 语言：[NodeJS](/windows/nodejs/setup-on-wsl2)、JavaScript、[Python](/windows/python/web-frameworks)、Ruby、C/C++、C# 和 F#、Rust、Go 等。
  - 服务：SSHD、[MySQL](./tutorials/wsl-database.md)、Apache、lighttpd、[MongoDB](./tutorials/wsl-database.md)、[PostgreSQL](./tutorials/wsl-database.md)。
- 使用自己的 GNU/Linux 发行版的软件包管理器安装其他软件。
- 使用类 Unix 的命令行 shell 调用 Windows 应用程序。
- 在 Windows 上调用 GNU/Linux 应用程序。
- [运行直接集成到 Windows 桌面的 GNU/Linux 图形应用程序](./tutorials/gui-apps.md)。
- [使用设备的 GPU 加速在 Linux 上运行的机器学习工作负载](./tutorials/gpu-compute.md)。

<a class="button button--primary" href="install">安装 WSL</a>

<div class="embeddedvideo"><iframe src="https://www.youtube-nocookie.com/embed/48k317kOxqg" frameborder="0" allowfullscreen="true" data-linktype="external" title="视频: 48k317kOxqg"></iframe></div>

## WSL 2 是什么？

WSL 2 是安装 Linux 发行版时的默认发行版类型。WSL 2 使用虚拟化技术在轻量级实用虚拟机 (VM) 中运行 Linux 内核。Linux 发行版作为 WSL 2 管理的 VM 中的隔离容器运行。通过 WSL 2 运行的 Linux 发行版将共享相同的网络命名空间、设备树 (除了 `/dev/pts` 之外)、CPU/内核/内存/交换（Swap）、`/init` 二进制文件，但具有自己的 PID 命名空间、Mount 命名空间、用户命名空间、Cgroup 命名空间和 `init` 进程。

相较于 WSL 1 的架构，WSL 2 **提高了文件系统性能**，并增加了 **完整的系统调用兼容性**。了解有关 [WSL 1 和 WSL 2 的比较](./compare-versions.md)。

独立的 Linux 发行版可以使用 WSL 1 或 WSL 2 架构运行。每个发行版都可以随时升级或降级，您可以同时运行 WSL 1 和 WSL 2 发行版。请参阅 [设置 WSL 版本命令](/windows/wsl/basic-commands#set-default-wsl-version)。

<div class="embeddedvideo"><iframe src="https://www.youtube-nocookie.com/embed/MrZolfGm8Zk" frameborder="0" allowfullscreen="true" data-linktype="external" title="视频: MrZolfGm8Zk"></iframe></div>

## Microsoft 热爱 Linux

了解有关 [Microsoft 的 Linux 资源](/linux) 的更多信息，包括在 Linux 上运行的 Microsoft 工具、Linux 培训课程、适用于 Linux 的云解决方案架构以及 Microsoft + Linux 的新闻、活动和合作伙伴关系。**Microsoft 热爱 Linux！**
