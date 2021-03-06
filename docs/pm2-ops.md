# pm2 运维经验

> 作者: UMU @ MEET.ONE 实验室

## 安装

比较多的文章推荐用 npm 安装，但 [UMU](https://blog.umu618.com/) 更推荐 yarn。

**理由**：[Visual Studio Code](https://code.visualstudio.com/) 脑残粉跟随 [Microsoft](https://github.com/Microsoft)/[vscode](https://github.com/Microsoft/vscode) 使用 yarn。

```
yarn global add pm2
```

## 运行

不熟悉 yarn 的话，装完一头雾水，装到哪了？用以下命令显示：

```
yarn global bin
```

结果参考：

- macOS：`/usr/local/bin`
- Ubuntu：`/home/ubuntu/.yarn/bin`

以 Ubuntu 为例，运行命令为：

```
/home/ubuntu/.yarn/bin/pm2 start my-program.js
```

## 安全建议

**root 身份能不用则不用。**
