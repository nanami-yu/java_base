# Strapi
> strapi 是一个先进的 Node.js 内容管理框架（headless-CMS），可以毫不费力地构建强大的 API

## 安装
### windows
> 参考地址 https://github.com/AutumnFish/strapi_study
```sh
npm install strapi -g
npx create-strapi-app test1
cd test1
npm install
npm run develop
```

### docker
```sh
docker pull strapi/strapi
# link到mysql数据库 并且需要创建持久化
docker run -d \
  --link=mysql \
  --name strapi \
  -e DATABASE_CLIENT=mysql \
  -e DATABASE_NAME=strapi_info \
  -e DATABASE_HOST=mysql \
  -e DATABASE_PORT=3306 \
  -e DATABASE_USERNAME=root \
  -e DATABASE_PASSWORD=123456 \
  -p 1337:1337 \
  -v /usr/local/strapi-docker/nanami:/srv/app \
  strapi/strapi
```

### 访问地址
192.168.1.162:1337

1@qq.com/1qaz@WSX

## 操作
> [中文文档](https://getstrapi.cn/)
>
> [简单操作](https://www.cnblogs.com/Frank-yafeya/p/14792567.html)