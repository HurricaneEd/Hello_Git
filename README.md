```bash
** 学习资源 **
https://liaoxuefeng.com/books/git/introduction/index.html

# 进入项目根目录
cd /path/to/your/project

# 初始化 Git 仓库
git init

# 添加所有文件到暂存区（缓冲区）
git add .

# 提交到本地仓库，-m 后跟提交说明
git commit -m "first commit"

# 添加远程仓库地址（请替换为自己的仓库地址）
# HTTPS 方式（无需配置 SSH）：
git remote add origin https://github.com/你的用户名/仓库名.git

# 或 SSH 方式（需提前配置 SSH 公钥）：
git remote add origin git@github.com:你的用户名/仓库名.git

# 首次推送，-u 建立本地 master/main 与远程的关联
git push -u origin master   # 若默认分支为 main，则使用 git push -u origin main

#后续代码更新
git add .                    # 添加修改
git commit -m "更新说明"      # 提交
git push                     # 推送（已关联后可省略远程和分支名）
