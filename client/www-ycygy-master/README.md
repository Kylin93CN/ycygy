# 杨超越公益官网

[官网地址](http://www.ycygy.cn/)

###  本地开发
```shell
yarn install
yarn run dev
```

###  发布
登陆阿里云
```shell
cd /home/ycygy/www-ycygy/
git pull
nuxt build
#使用pm2
pm2 start npm --name "cygy-www" --watch  -- run start
```
