# Hexo github配置教程
#### 准备材料：
1. 安装node
2. Github SSH Key
#### 步骤
(教程)[https://zhuanlan.zhihu.com/p/22098309?utm_source=wechat_session&utm_medium=social&utm_oi=52770035990528]
1. 创建repo，命名方式必须为：<username>.github.io, 如：soonyenju.github.io， clone到本地
2. npm install -g hexo-cli
3. cd soonyenju.github.io
4. npm install
5. 本地运行测试：hexo s
6. 生成js等文件：hexo g
7. 配置_config.yml准备部署
'''
deploy:
 type: git
 repo: git@github.com:soonyenju/soonyenju.github.io.git
 branch: master
'''
注意：1. 必须用space，不能用tab，而且空格不能多也不能少！
8. 安装hexo-deployer-git： npm install hexo-deployer-git --save
9. 部署：hexo d -g

#### 踩坑
[attempting to use a Jekyll theme](https://www.jianshu.com/p/fb0cb9affe19?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation)
[The tag `fancybox` on line 77 in `themes/landscape/README.md` is not a recognized Liquid tag.](https://www.jianshu.com/p/fb0cb9affe19?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation)