# 配置环境
首先，确保你已经安装了Node.js和Express。然后创建一个新的目录，进入该目录，并在命令行中运行以下命令来初始化一个新的Node.js项目：

npm init -y

然后，安装Express：

npm install express

# 解决跨域问题
npm install cors


然后，在你的Express应用中添加以下代码来启用CORS中间件：
const express = require('express');
const cors = require('cors');
const app = express();

// 允许来自所有域名的请求
app.use(cors());

// 其他路由和中间件的定义

这样，Express应用将允许来自任何域名的请求，并自动处理跨域请求的相关头部信息。
