# 操作手册

打开仓库根目录的 `test.md`，应看到一行 `test done`。

修改后推送 feature 分支并提交 PR，在 GitHub 的 Actions 或 PR 检查页面查看 `Check test.md` 的结果。检查要求文件内容恰好为 `test done`，末尾带一个换行。

仓库原先没有测试或 CI，本次新增远端文件内容检查，不需要编译。不要在本地运行构建、编译测试或冒烟脚本。
