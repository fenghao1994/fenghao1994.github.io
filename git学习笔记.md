## GIT

### git 日志方面命令
- git log -p 查看每个commit提交的细节(-p -> --patch)
- git log --stat 查看简要统计,统计出来的是哪些文件修改哪些几处 -> 方便查看在哪个commit中修改了哪个文件。 
- git show 查看当前的commit的提交内容细节(-p 是可以查看全部) ，也可以利用  git show "SHA-1(commit的sha-1值)" 查看具体的一个commit的具体细节，还可以利用 git show "SHA-1" "file name(文件名)" 查看具体的文件的修改详情

### git 修改对比(diff)
- git diff --staged(与 git diff --cache 命令作用相同)(显示暂存区和上一条提交之间的不同, 相当于输入 git commit之后的修改)
- git diff (没有参数) 显示工作目录和暂存区之间的不同(相当于输入git add . 之后的提交)
- git diff HEAD (显示工作目录和上一条提交之间的不同) (HEAD 可以换成其他commit，这样可以看到和其他commit的不同)
 