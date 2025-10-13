# Git与GitHub入门教程教案

## 一、课程基本信息
- 课程名称：Git与GitHub版本控制基础
- 授课对象：主要为大一新生
- 课时：2课时（理论1课时+实操1课时）
- 教学环境：带电脑的多媒体教室，确保网络通畅

## 二、教学目标
1. 理解版本控制的基本概念及重要性
2. 掌握Git的核心原理和基本操作
3. 学会使用VSCode图形化界面操作Git
4. 能够使用GitHub管理个人项目和参与团队协作
5. 了解开源项目参与方式和GitHub Actions基础

## 三、教学重点与难点
- 重点：Git的基本操作（提交、分支、合并）、GitHub项目管理
- 难点：Git的工作原理、分支概念、协作流程

## 四、教学准备
1. 教师准备：
   - 示例代码仓库（含基础项目结构）
   - 演示用幻灯片
   - 操作步骤文档
   - 课堂练习任务单

2. 学生准备：

**不要把软件安装在C盘**

   - 安装Git（https://git-scm.com/downloads）（在安装过程中勾选“使用VSCode作为Git的默认编辑器”，其他默认）
   - 安装VSCode（https://code.visualstudio.com/）（安装中文插件）
   - 注册GitHub账号（https://github.com/join）（注册一个简短的英文用户名）

   完成以上任务后在飞书收集表中填写姓名、Github用户名、`git --version`命令的运行结果截图、中文界面的VSCode截图
 
## 五、教学过程

### 第一部分：导入（10分钟）

**活动1：日常文档管理问题讨论**
- 提问学生："大家平时写论文或报告时，如何保存不同版本？"
- 展示常见问题：
  - 多个文件版本混乱（如：论文_final.docx、论文_final_v2.docx）
  - 误删内容无法恢复
  - 多人协作时文件传递麻烦
  - 想恢复到之前的版本困难

- 引出主题：Git正是为解决这些问题而设计的版本控制系统

### 第二部分：Git基础理论（30分钟）

**1. 什么是版本控制**
- 定义：记录文件内容变化，以便将来查阅特定版本修订情况的系统
- 优势：
  - 回溯到任意历史版本
  - 多人协作更高效
  - 可以并行开发不同功能
  - 错误恢复更简单

**2. Git核心概念**
- 工作区（Working Directory）：本地电脑上的项目文件夹
- 暂存区（Staging Area）：临时存放改动的地方
- 版本库（Repository）：存放所有版本信息的数据库

**3. Git工作流程**
- 图形演示：工作区 → 暂存区 → 版本库的流程
- 在Git中配置Github用户名以及和用户名对应的邮箱（命令行完成）
- 核心操作（通过VSCode图形化界面完成）：
  - `git init`：初始化一个新的Git仓库
  - `git clone`：克隆远程仓库到本地
  - `git status`：查看当前工作区和暂存区状态
  - `git add`：将工作区的改动添加到暂存区
  - `git commit`：将暂存区的内容提交到版本库
  - `git push`：将本地版本库的内容推送到远程仓库

**4. 分支概念**
- 比喻：如同树枝从树干生长，分支允许并行开发
- 主分支（main/master）：稳定的主版本
- 功能分支（feature branch）：开发新功能时使用
- 演示分支创建、切换和合并的流程

### 第三部分：VSCode中使用Git（25分钟）

**1. VSCode Git界面介绍**
- 侧边栏Git图标位置
- 主要功能区域：更改、暂存、提交历史等

**2. 实操演示：创建第一个本地仓库**
- 步骤1：创建新项目文件夹
- 步骤2：在VSCode中打开文件夹
- 步骤3：初始化仓库（Initialize Repository）
- 步骤4：创建文件并添加到暂存区
- 步骤5：填写提交信息并提交
- 步骤6：查看提交历史

**3. 分支操作演示**
- 创建新分支
- 在新分支上修改文件
- 切换回主分支查看差异
- 合并分支

### 第四部分：GitHub使用（35分钟）

**1. GitHub简介**
- 定义：基于Git的代码托管平台
- 用途：项目存储、版本管理、协作开发

**2. 远程仓库操作**
- 演示：在GitHub上创建新仓库
- 连接本地仓库与远程仓库
- 推送本地代码到GitHub（push）
- 从GitHub拉取最新代码（pull）

**3. 个人项目管理的最佳实践**
- README文件的重要性
- 项目结构组织
- 使用.gitignore忽略不需追踪的文件

**4. 团队协作基础**
- 邀请协作者
- Issues功能：跟踪问题和任务
- Pull Request（PR）：提交修改请求
- Code Review：代码审查流程

**5. 参与开源项目**
- 搜索感兴趣的开源项目
- Fork项目
- 提交PR的流程
- Star和Watch功能

**6. GitHub Actions简介**
- 自动化流程的概念
- 常见用途：自动测试、自动部署
- 简单示例展示

### 第五部分：课堂实操（40分钟）

**任务1：创建个人仓库**
- 在GitHub上创建仓库名为你的用户名的公共仓库
- 克隆到本地
- 添加/编辑自我介绍文件
- 提交并推送到远程

**任务2：参与示例仓库**
- 访问社团组织提供的示例仓库
- 提交一个Issue（可以是学习/技术/校园生活遇到的问题，或是对网协授课的意见建议）
- Fork仓库并添加你的自拍照或二次元头像
- 提交Pull Request

### 第六部分：课堂小结与作业（10分钟）

**课堂小结**
- 回顾Git的核心概念和工作流程
- 强调GitHub在协作中的作用
- 鼓励学生在今后的学习中积极使用版本控制

**课后作业**
1. 完善课堂上创建的个人简介仓库
2. 找到一个感兴趣的开源项目，Star并Watch

## 六、教学评估
- 课堂实操完成情况
- 提交的Issue和PR质量

## 七、教学反思（课后填写）
- 学生对哪些概念理解困难
- 实操环节中出现的共性问题
- 下次教学可以改进的地方

## 八、补充资源

**读官方文档！！！**

**学英文或使用沉浸式翻译**

- Git官方文档：https://git-scm.com/doc
- GitHub Learning Lab：https://lab.github.com/
- VSCode Git教程：https://code.visualstudio.com/docs/editor/versioncontrol
- Github Profile官方文档：https://docs.github.com/en/account-and-profile/how-tos/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme
- Github Page官方文档：https://docs.github.com/en/pages/quickstart