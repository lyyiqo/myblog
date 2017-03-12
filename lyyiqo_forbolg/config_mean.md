介绍配置文件的网站：
http://chping.website/2016/08/31/Hexo1/


# Hexo Configuration
## Docs: https://hexo.io/docs/configuration.html
## Source: https://github.com/hexojs/hexo/
# Site                                   ##站点配置
title: 前端小开发                         ##站点名称,一级标题
subtitle: 随笔 分享 笔记 			 ##站点二级标题
description: 分享前端技术 整理学习笔记     ##站点简介（个人简介）
author: 彬仔                             ##站点博主昵称
avatar: /images/avatar.png               ##站点博主头像（自定义添加的，照片存放在source/images路径下）
language: zh-Hans                        ##站点语言
timezone: Asia/Hong_Kong                 ##站点时区
# URL  ##网址
## If your site is put in a subdirectory, set url as 'http://yoursite.com/child' and root as '/child/'
## 如果您的网站存放在子目录中，例如 http://yoursite.com/blog，则请将您的 url 设为 http://yoursite.com/blog 并把 root 设为 /blog/。
url: https://chping2125.github.io/    ##没有子目录则设置为username.github.io(资源的引用会将该URL拼在资源路径前面)
root: /
permalink: :year/:month/:day/:title/  ##如果有子目录生成文件名字的格式我改成blog/:title:year:month:day/，否则不改
permalink_defaults:

# Directory                  ##资源目录配置
source_dir: source           ##站点资源文件夹（即Hexo的文件目录中source文件夹）
public_dir: public           ##站点公共文件夹（这个文件夹用于存放生成的站点文件，一般为临时文件"hexo g"命令后会生成，“hexo clean”命令会删除该文件）
tag_dir: tags                ##标签文件夹
archive_dir: archives        ##归档文件夹
category_dir: categories     ##分类文件夹
code_dir: downloads/code     ##nclude code 文件夹
i18n_dir: :lang              ##国际化（i18n）文件夹
skip_render: README.md       ##跳过指定文件的渲染，您可使用 glob 表达式来匹配路径。(GitHub中的README.md就配置在这里，防止渲染)
# Writing   ##博客文章
new_post_name: :title.md # File name of new posts  ##默认文章名称
default_layout: post                               ##默认文章布局样式
titlecase: false                                   ##小写文章标题
external_link: true                                ##在新标签中打开一个外部链接，默认为true
filename_case: 0  ##转换文件名，1代表小写；2代表大写；默认为0，意思就是创建文章的时候，是否自动帮你转换文件名，默认就行，意义不大。
render_drafts: false                               ##是否渲染_drafts目录下的文章，默认为false
post_asset_folder: false                           ###启动 Asset 文件夹
relative_link: false                               ##把链接改为与根目录的相对位址，默认false
future: true                                       ##显示未来的文章，默认false
highlight:                                         ##代码块的设置
  enable: true                        ##默认开启
  line_number: true                   ##行号，默认开启
  auto_detect: false                  ##自动检测
  tab_replace:
# Category & Tag                      ##分类和标签的设置
default_category: uncategorized       ##默认分类
category_map:                         ##分类别名
tag_map:                              ##标签别名
# Date / Time format 
## Hexo uses Moment.js to parse and display date
## You can customize the date format as defined in
## http://momentjs.com/docs/#/displaying/format/
date_format: YYYY-MM-DD
time_format: HH:mm:ss
# Pagination ##分页
## Set per_page to 0 to disable pagination
per_page: 10          ##每页显示的文章量 (0 = 关闭分页功能)
pagination_dir: page  # #分页目录
# Extensions        ##主题设置
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: next         ##主题名称
# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:            ##部署地址github设置
  type: git        ## 部署的位置  写git
  repository: git@github.com:chping2125/chping2125.github.io.git 
  ## 这里填写项目的地址 git@github.com:Git用户名/Git用户名.github.io.git 参照上面
  branch: master   ## 分支选择 master
####自定义第三方插件
# Share      ##博客文章分享功能
##Duoshuo_Share       ##多少分享
duoshuo_shortname: chping    ##就是在多少设置的站点名称
duoshuo_share: true 
##JiaThis_Share       ##JiaThis分享
jiathis: false 
##baidu_Share         ##百度分享
baidushare: false
#BaiDu_Analytics      ##百度分析
baidu_analytics: c8027b8ba4beebe6ebe89d22781de0a1 
##search              ##搜索功能
search:
  path: search.xml
  field: post