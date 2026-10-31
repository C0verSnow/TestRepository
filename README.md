# TestRepository

## Issue #8

[Issue #8](https://github.com/C0verSnow/TestRepository/issues/8) 要求在仓库根目录新增 [Issuetest.md](Issuetest.md)，内容为单行 `issue test done`，行末保留换行。

## 检查方式

[GitHub Actions](.github/workflows/issue-test.yml) 在 push、pull_request 或手动触发时，检查 `Issuetest.md` 是否与预期内容完全一致，包括大小写和行末换行；文件缺失或内容不同都会导致检查失败。检查只读取文件，不会自动生成或修复文件。

遵守项目约定，不在本地编译或运行测试。远端 CI 结果由后端在发布后核实，当前不声称已通过。后端负责提交、推送和创建或更新 PR，并在 CI 通过后按 after_ci 策略关闭 Issue；PR 保持 Open，等待用户 Review。

执行过程见 [tasklist.md](tasklist.md)。
