# vvsMarkdown
Electron+React+七牛云 实现跨平台桌面级应用
# Electron 主进程 - 负责创建窗口，提供原生应用的各种模块
    Electron 渲染进程 - 提供浏览器环境
        React 作为View层完成各种交互
        Node.js 负责本地文件的创建管理，网络文件的下载等
        七牛云对象存储 负责本地文件同步到云端，提供上传下载的服务

# 配置开发环境
    创建react文件：npx create-react-app [filename...]
    添加依赖：npm install electron --save-dev （将react集成到electron中）
             npm install electron-is-dev --save-dev (用来判断是生产环境还是开发环境)
             npm install concurrently --save-dev (并发执行npm命令)
             npm install wait-on --save-dev (用来等待某个file/ports/sockets/https资源释放)
             npm install cross-env --save-dev (用来解决跨平台的环境变量设置问题))
             nom install bootstrap --save (添加样式库)
