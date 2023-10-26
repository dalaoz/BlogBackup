## Blog备份

方便他人，方便自己，喜欢的点个Star

**关于主题：**

1. 崇尚简约
2. 追求移动端体验
3. 希望把加载速度做到极致（努力中）
4. 让大家把注意力放到内容上。这是本主题设计初衷
5. 主题不支持IE6，7，8。以后也不会
6. 2023/10/24重大更新
7. 去除了统计、以及各种绑定，几乎秒开

### 1 使用方法

​	首先本地现有`Git`、`NodeJS`、`Python`（网络上安装方法一大堆，或者催更我出一个教程）

```bash
# 以下是我的版本 2023/10/24
PS C:\DaLao\Desktop> git --version
git version 2.42.0.windows.2

PS C:\DaLao\Desktop> node -v
v18.18.2
PS C:\DaLao\Desktop> npm -v
9.8.1

PS C:\DaLao\Desktop> python --version
Python 3.12.0
```

​	1、安装完以上环境后安装[Hexo](https://hexo.io/zh-cn/docs/)：

```bash
# 这是全局安装，有自己想法的可以去官方Docs
npm install -g hexo-cli
```

​	2、在桌面新建一个文件，该文件将是你的博客目录

```bash
# 目录初始化
hexo init
```

注意：这里必须是Git命令状态使用`hexo`

![image-20231025225633487](https://img-date.oss-cn-hangzhou.aliyuncs.com/img/202310252316484.png)

​	初始化后，会出现很多文件。除了`node_modules`，其他全部删除

![image-20231025232131826](https://img-date.oss-cn-hangzhou.aliyuncs.com/img/202310252321633.png)

​	3、然后下载我的Github备份

```bash
# 拉去我的博客bei'feng
git clone https://github.com/dalaoz/BlogBackup.git
```

```bash
# 安装我的依赖
npm install
```

新的目录结构如下：

```bash
.
├── _config.yml	# 博客主要配置文件
├── ImageProcess.py	# 修剪图片调用，不要动
├── tool.py	# 修剪图片脚本
├── node_modules	# hexo博客依赖的模块
├── min_photos	# 相册缩略图
├── photos	# 原图
├── package.json # npn install 需要安装的依赖列表					
├── package-lock.json	# npn install 依赖的模块安装记录
├── scaffolds	# 模版文件夹
├── source	# 文章存放
├── themes	# 主题文件夹
│   └── yilia	# 主题
│       ├── _config.yml	  # 主题主要配置文件
│       └──...	
└── README.md # 说明文件
```

​	4、启动

```bash
# 启动hexo
hexo s

# 打开网址
http://localhost:4000/
```

![image-20231026214648089](https://img-date.oss-cn-hangzhou.aliyuncs.com/img/202310262146984.png)

### 2 我很懒

看Issues里面问题多不多，多的话，我会更新一下！

### 3 另外

相册：脚本修改过的图片，我选择放在阿里云的OSS里面。有问题请私信！
