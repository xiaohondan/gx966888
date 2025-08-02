# gx966888
gx966888安装工具
使用示例
# 添加一个工具仓库
repo-install add https://github.com/johnsmith/awesome-cli-tool.git

# 添加另一个仓库
repo-install add https://gitlab.com/devteam/productivity-suite.git

# 列出所有仓库
repo-install list
# 输出:
# 📋 Stored repositories:
# https://github.com/johnsmith/awesome-cli-tool.git
# https://gitlab.com/devteam/productivity-suite.git

# 安装工具（交互式选择）
repo-install install
# 输出:
# 1) https://github.com/johnsmith/awesome-cli-tool.git
# 2) https://gitlab.com/devteam/productivity-suite.git
# 选择要安装的仓库: 1
# 📦 Cloning repository...
# 🔧 Found install script
# ...
# ✅ Installation complete!
工具特点
跨平台支持：

自动检测系统类型（APT/YUM/DNF/Pacman）

安装必要的Git依赖

灵活的安装方式：

支持 install.sh 自定义脚本

支持 Makefile 安装

支持 .deb/.rpm 包自动安装

仓库管理：

永久存储仓库地址在 ~/.repo-installer.conf

交互式安装菜单

清晰的列表展示

安全隔离：

在临时目录操作

安装后自动清理

这个解决方案让您只需记住一个命令 repo-install，就能管理所有工具仓库的安装。需要您指定的就是各个工具的实际仓库地址，其余所有过程都会自动完成。
