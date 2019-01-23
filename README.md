# 国民心理健康素养评估与促进 - 网站源码

## 工具

- node 8.12.0 (npm 6.4.1)
- Hexo 3.8.0
- Hexo-cli 1.1.0
- 主题：NexT

## 内容架构

- `source`: 内容源，包含文字、图片
- `global_config.yml`: Hexo 全局配置文件
- `next_config.yml`: Hexo 主题 NexT 配置文件

## 使用方法

下述命令均指在系统终端运行，并假设命令行开始时用户在网站文件夹的父目录下。

使用下述命令新建一个 Hexo 目录：

```
mkdir blog
cd blog
hexo init
```

使用主题 NexT：

```
cd blog
git clone https://github.com/theme-next/hexo-theme-next themes/next
```

直接覆盖 `source` 以修改内容。

使用下述命令生成静态文件：

```
cd blog
hexo clean
hexo generate
```

将生成的 `public/*` 覆盖掉 master 分支下的内容后，为自定义首页创建软链接：

```
ln -s index/index.html index.html
```

然后更新到远端即可
