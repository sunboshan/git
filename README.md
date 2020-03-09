## git

`oh-my-zsh`的git plugin中最常用的git命令。方括号中为`tig`的快捷方式。

```
$ cat ~/.oh-my-zsh/plugins/git/git.plugin.zsh

# -------
# 常用
# -------

$ gss           [s]                        # 列出文件修改状态
$ gaa/gau       [u]   status-view          # 添加文件
$ gd/gds        [o]   status-view          # 查看修改
$ gcmsg         [C|1] status-view          # 提交修改
$ glol/glola    [m]                        # 查看历史

# -------
# 修改
# -------

$ gc!           [+] status-view            # 修改最近的commit(清空commit msg可以取消)

# -------
# 重置
# -------

$ grh           [u] status-view            # 重置gaa
$ grhh          [!] status-view            # 重置所有修改(慎用!)
$ groh                                     # 重置所有修改至远程分支(慎用!)
$ gclean        [-] status-view            # 删除未跟踪文件

# -------
# 暂存
# -------

$ gstl          [y]                        # 列出暂存
$ gsts                                     # 显示暂存
$ gsta/gstall                              # 保存暂存
$ gstp                                     # 弹出暂存
$ gwip                                     # 提交所有修改到wip
$ gunwip                                   # 撤销wip

# -------
# 分支
# -------

$ gb            [r]                        # 本地分支
$ gbr           [r]                        # 远程分支
$ gbd/gbD       [d|D] refs-view            # 删除分支
$ gco           [c]   refs-view            # 切换分支/重置文件
$ gcb           [B]   main-view            # 新建分支并切换

# -------
# 远程
# -------

$ ggsup                                    # 跟踪远程
$ ggl/gl                                   # 拉最新代码
$ ggp           [P] main-view              # 推本地代码
$ gfa                                      # 同步远程

# -------
# 变基
# -------

$ ggu           [U] main-view              # 拉最新代码并且变基
$ grbi          [S] main-view              # 手动变基
$ grbc                                     # 继续变基

# -------
# 配置
# -------

$ gcf                                      # 显示配置
```
