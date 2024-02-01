# Veeam 加固存储库 

这个Linux脚本根据Veeam官方的加固建议[Veeam Hardened Linux Repository](https://helpcenter.veeam.com/docs/backup/vsphere/hardened_repository.html?ver=120)对Ubuntu 20.04系统进行自动化加固，在使用我的[加固存储库自动配置脚本](https://github.com/Coku2015/Veeam_Repo_Configurator)创建完存储库后，可以用本脚本对Ubuntu系统进行进一步自动加固。

本脚本根据VeeamHub/veeam-hardened-repository的DISA STIG脚本进行修改，适合中国用户加固Ubuntu 20.04系统。

这个工具并非Veeam官方支持的产品，如有任何问题，请联系lei.wei@veeam.com

## 📗 文档

**系统要求:**

- 必须以root用户身份运行
- 必须在一台干净安装的Ubuntu 20.04系统上运行
- 仅支持 Veeam Backup & Replication v12 以上版本

**使用说明:**

1. 通过 SSH 连接到 Ubuntu 20.04 服务器上
2. 复制脚本内容到该服务器上
3. 使用以下命令运行脚本:
```bash
sudo bash veeam.harden.sh > output.txt 2>&1
```

注意: 如果你需要更详细的输出，只需运行以下的命令:
```bash
sudo bash veeam.harden.sh
```

## 🤝🏾 License

* [MIT License](LICENSE)

