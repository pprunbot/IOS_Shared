# 项目部署  

## 准备
- 克隆项目到本地  
- 下载[node.js](https://nodejs.org/zh-cn)
- 修改<kbd>.env</kbd>中的api地址和域名地址
~~~
VITE_API_URL=小火箭账号API
VITE_APP_DOMAIN=网站域名，用于访问统计
~~~
- 小火箭API的返回格式示例
~~~
{
    "id": [
        {
            "id": "123748123",
            "email": "xhjid@id.com",
            "password": "qwer1234",
            "status": "正常"
        },
        {
            "id": "238713123",
            "email": "qqweee@id.com",
            "password": "1234qwer",
            "status": "异常"
        }
    "message": "获取成功"
}
~~~
- 访问统计采用的项目[Webviso：基于Clouflare+D1的web访客统计服务](https://webviso.yestool.org/)

## 打包  
~~~
npm i
npm run build
~~~

## 部署
- 将生成的dist目录下的文件复制到你的网站根目录即可
