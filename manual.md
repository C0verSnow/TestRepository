# 使用说明

打开仓库根目录的 `tgtest.md`，应看到一行文字：

```text
tg test success
```

提交或 PR 到 main 分支后，GitHub Actions 的“检查任务文件”会检查文件是否存在，以及内容是否与上述文字一致（末尾保留换行）。在 PR 的 Checks 页面查看结果。该检查不需要编译。
