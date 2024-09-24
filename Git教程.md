# Git/Github使用教程

## 一、入门视频

- github网页使用

[【『教程』一看就懂！Github基础教程】]([『教程』一看就懂！Github基础教程_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1hS4y1S7wL/?share_source=copy_web&vd_source=7a007e4f564788534f2a868e13842e19))

- github deskstop

[【教程】GitHub Desktop管理你的项目](https://www.bilibili.com/video/BV13W411U7HY/?spm_id_from=333.788.recommend_more_video.-1&vd_source=47fc0cc04a21237719f0c5d6fe89d40e)



## 一、初识Git

- [『教程』简单明了的Git入门_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Cr4y1J7iQ/?share_source=copy_web&vd_source=7a007e4f564788534f2a868e13842e19))

（视频中的教程是针对于使用命令进行管理）

#### 1. 什么是 Git？

Git 是一种分布式版本控制系统，可以帮助你跟踪代码的历史记录、管理项目中的不同版本，以及与团队成员协作开发。使用 Git，你可以保存不同的版本，方便回溯或协同工作。

#### 2. 什么是 GitHub 和 GitHub Desktop？

- **GitHub** 是一个基于 Git 的代码托管平台，允许开发者远程托管代码并与其他人协作开发。
- **GitHub Desktop** 是一个图形化的 Git 客户端，可以让你在不使用命令行的情况下轻松管理代码仓库，尤其适合 Git 新手。

## 二、GitHub Desktop 安装与使用

[GitHub Desktop使用教程-CSDN博客](https://blog.csdn.net/qqw666666/article/details/125652869?ops_request_misc=%7B%22request%5Fid%22%3A%22AAE1E5EC-CF74-437E-BAA7-C03F50B87FA2%22%2C%22scm%22%3A%2220140713.130102334..%22%7D&request_id=AAE1E5EC-CF74-437E-BAA7-C03F50B87FA2&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~baidu_landing_v2~default-1-125652869-null-null.142^v100^pc_search_result_base1&utm_term=github deskstop使用教程&spm=1018.2226.3001.4187)

#### 2.1 安装 GitHub Desktop

1. 访问 [GitHub Desktop 官方网站](https://desktop.github.com/)。
2. 根据你的操作系统下载并安装 GitHub Desktop。

#### 2.2 配置 GitHub Desktop

1. 安装后启动 GitHub Desktop，首次使用时会提示你登录 GitHub 账号。你可以使用 GitHub 账号登录或创建一个新账号。GitHub官网：https://github.com/
2. 登录成功后，可以在主界面中看到项目仓库管理的相关选项。

#### 2.3 基本功能介绍

GitHub Desktop 的主要功能包括：

- **Clone a Repository（克隆仓库）**：从 GitHub 上下载已有的仓库到本地。
- **Create a New Repository（创建新仓库）**：在本地创建一个新的 Git 仓库并将其与 GitHub 同步。
- **Add an Existing Repository（添加现有仓库）**：将本地已有的 Git 仓库导入到 GitHub Desktop 中进行管理。

#### 2.4 GitHub Desktop 基本使用流程

##### 1. 克隆远程仓库到本地

如果你想要将 GitHub 上的项目下载到本地，可以执行以下步骤：

1. 在 GitHub Desktop 中点击 **File > Clone Repository**。
2. 选择想要克隆的仓库，然后点击 **Clone**。

##### 2. 创建本地仓库并同步到 GitHub

1. 点击 **File > New Repository**，创建一个新的本地仓库。
2. 选择本地路径并填写仓库名称。
3. 创建完仓库后，点击 **Publish Repository**，将本地仓库同步到 GitHub。

##### 3. 提交（Commit）更改

1. 修改或新增项目中的文件后，回到 GitHub Desktop，会看到 **Changes** 栏目下列出了所有的更改。
2. 输入提交信息，并点击 **Commit to main**，将更改提交到本地仓库。

##### 4. 推送（Push）到远程仓库

在本地提交后，你需要将更改推送到 GitHub 上的远程仓库：

1. 点击 **Push origin**，将提交的更改推送到 GitHub 上。

##### 5. 拉取（Pull）远程仓库的更改

当远程仓库有其他人提交的更改时，你可以拉取最新的代码到本地：

1. 点击 **Fetch origin** 检查是否有新的更改。
2. 如果有，点击 **Pull origin** 拉取最新的更改。

#### 2.5 分支管理

GitHub Desktop 也支持分支的创建和管理，帮助你更好地组织代码：

1. 在主界面中点击 **Current Branch**，然后选择 **New Branch** 创建新的分支。
2. 在分支上做更改并提交后，可以通过 **Merge into Current Branch** 将分支合并到主分支。

---

### 三、常用 Git 命令对比 GitHub Desktop 操作

| Git 命令              | GitHub Desktop 操作       | 说明                |
| --------------------- | ------------------------- | ------------------- |
| `git init`            | File > New Repository     | 初始化本地 Git 仓库 |
| `git clone <url>`     | File > Clone Repository   | 克隆远程仓库到本地  |
| `git add .`           | 自动检测文件更改          | 添加文件到暂存区    |
| `git commit -m "msg"` | Commit to main            | 提交更改            |
| `git push`            | Push origin               | 推送更改到远程仓库  |
| `git pull`            | Pull origin               | 拉取远程仓库的更改  |
| `git branch <branch>` | New Branch                | 创建新分支          |
| `git merge <branch>`  | Merge into Current Branch | 合并分支            |

---

### 四、常见问题

#### 1. 本地提交后无法推送到远程仓库？

确保你已经正确设置了远程仓库 URL，并且你有权限向远程仓库推送。如果在 GitHub Desktop 中，点击 **Repository > Repository Settings**，检查远程仓库设置。

#### 2. 如何处理冲突？

当多个开发者同时修改了同一文件并提交时，可能会产生冲突。你需要手动解决这些冲突后再提交和推送。

---

