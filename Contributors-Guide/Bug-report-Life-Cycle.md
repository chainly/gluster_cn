本页面描述了生活的一个 bug 报告。

-当第一次报告的 bug，它给 * * 新 * * 地位。
-一旦开发人员已经开始或规划工作上的错误，
地位 * * 分配对象 * * 设置。"分配给"字段应提

特定的开发人员。
-如果一个初步
[补丁](https://en.wikipedia.org/wiki/Patch _(computing)) 的 bug

已投入 [Gerrit 代码审查
工具] (http://review.gluster.org)，地位 * * 应设置邮政 * *
手动。地位 * * 邮政 * * 应仅使用时的所有修补程序

为某一特定 bug 已过帐的审查。
-此修补程序，并传递任何审查后自动回归
测试，此修补程序将得到合并由维护人员之一。当

修补程序已并入 git 仓库，被添加注释
该 bug。只有当所有需要的修补程序已经合并，分配

工程师将需要将状态更改为 * * * * 修改时间。
-后一套，可修复该 bug 的状态应该
移动到 * * ON\_QA * *。
-* * 固定版本 * * 领域应该得到的工作做一个名称释放
包含此修复程序的包。多个包

通常可用分布将获得后的几天内
* 使 dist * tar 文件被创建。
-这告诉 bug 记者包是提供解决问题的方法
为 bug，那他们应该测试包。
-释放维护人员需要做这种变化对 bug 状态
脚本是可用 (问 * ndevos *)。
-状态 * * 验证 * * 设置如果 QA 测试人员或者记者
确认此修复程序后的解决方法是合并后，新生成的修复
解决了问题。
-如版本不能解决报告的 bug，状态应该
退到 * * 分配对象 * * 带有明显确切注意什么
失败。
-当解决了一份报告，它给 * * 关闭 * * 地位。这

可以的意思是︰
-* * 关闭 / NEXTRELEASE * * 当通过代码改变这
已合并报告的主线问题的修补程序。
-* * 关闭 / CURRENTRELEASE * * 时，修复了代码更改
报告的 bug 已在相应的发布分支合并
和一个版本发布的修复。
-* * 关闭 / WONTFIX * * 报告的问题或建议时
有效的但报告的问题或执行任何修复
建议将禁止审批通过的项目
开发人员/维护者 （或产品经理，如果存在）。
-* * 关闭 / WORKSFORME * * 时不能重现该问题，
当尚未提供缺少的信息，或
可接受变通办法来实现类似的结果
要求。
-* * 关闭 / CANTFIX * * 当问题不是一个 bug，或当它是
GlusterFS 发展的权力范围以外的变化。为

示例中，提出对第三方软件更改的 bug 不能
固定在 GlusterFS 项目本身。
-* * 关闭 / 重复 * * 时这个问题之前，已有报告
不管前一份报告已经解决或
不。

如果一个 bug 报告被标记为 * 闭 * 或 * 验证 * 和它原来
这是不对的 bug 可以更改为地位 * 分配对象 *
或 * 新 *。
