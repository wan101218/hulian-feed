# hulian-feed

PC 端 DSH 与手机端 DSH 之间「按需同步」的**公开加密镜像**。

这里只有 AES-256-GCM 加密后的同步包密文，没有明文内容；
解压需要口令，口令不在本仓库里。

下载与导入（手机端）：

```bash
node hulian-pull.mjs --repo wan101218/hulian-feed --public --import \
  --target <工作区> --dsh-home <DSH 数据目录>
```

口令从 `--passphrase`、环境变量 `HULIAN_PASSPHRASE` 或 `~/.hulian-pass` 读取。
