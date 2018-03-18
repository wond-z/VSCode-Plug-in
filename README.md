# VSCode-Plug-in
## 离线下载vscode插件方式

[官方说明地址](https://code.visualstudio.com/docs/editor/extension-gallery?pub=HookyQR&ext=beautify#_common-questions)

**下载插件方式**

插件下载地址：

```
https://marketplace.visualstudio.com/vscode
```

使用以下拼接地址：

```
http://${publisher}.gallery.vsassets.io/_apis/public/gallery/publisher/${publisher}/extension/${extension name}/${version}/assetbyname/Microsoft.VisualStudio.Services.VSIXPackage
```

例如：

```
http://abusaidm.gallery.vsassets.io/_apis/public/gallery/publisher/abusaidm/extension/html-snippets/0.2.1/assetbyname/Microsoft.VisualStudio.Services.VSIXPackage
```

**安装方式**

使用‘从VSIX安装...’

## ssh配置

1.在用户文件夹下创建 `.ssh` 目录
```
mkdir .ssh
```

2.执行以下命令
```
ssh-keygen -t rsa -C "xxxxxx@yy.com"  #建议填写自己真实有效的邮箱地址,一路回车
```

3.打开 `id_rsa.pub` 文件，复制公钥并粘贴到GitHub中 `New an SSH key` 的key输入框

4.配置账户
```
# 设置用户名
$ git config --global user.name "your_username"

# 设置邮箱地址(建议用注册giuhub的邮箱)
$ git config --global user.email "your_registered_github_Email"
```