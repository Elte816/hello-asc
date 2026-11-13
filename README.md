# hello-asc · Git & GitHub 训练仓库

ASC 新人培训用。练完这个仓库，你就掌握了团队协作的标准 Git 工作流。

## 仓库内容

| 文件 | 说明 |
|---|---|
| `pi_serial.c` | 蒙特卡洛法估算圆周率（串行版）——训练用示例代码 |
| `MEMBERS.md` | 成员名单——课后任务的目标文件 |

## 课后任务：把你的名字加进名单（Fork + PR 流程）

1. **Fork** 本仓库到你的账号（右上角 Fork 按钮）
2. **Clone** 你 fork 后的仓库到本地：
   ```bash
   git clone https://github.com/你的用户名/hello-asc.git
   cd hello-asc
   ```
3. **修改** `MEMBERS.md`：按表格格式添加一行你的信息
4. **提交并推送**：
   ```bash
   git add MEMBERS.md
   git commit -m "名单添加：你的名字"
   git push
   ```
5. **提 Pull Request**：回到你的 fork 页面，点击 **Compare & pull request**，填写标题后提交
6. 等待组织者合并。合并完成后，刷新本仓库的 `MEMBERS.md` 就能看到你的名字 🎉

## 进阶挑战（选做）

- 试着把 `pi_serial.c` 用 OpenMP 并行化（提示：`#pragma omp parallel for` + `reduction(+:inside)`），比较一下 50 亿个采样点时串行和并行的耗时
- 在你的 fork 里新建一个 `optimizations.md`，记录你尝试过的优化手段和效果——这正是 ASC 初赛期间组织队伍优化记录的好习惯
