# 系统做成
## 1、安装相关包
- **Go开发及Debug调试工具**
    ~~~ commandline
    go install github.com/go-delve/delve/cmd/dlv@latest
    go install honnef.co/go/tools/cmd/staticcheck@latest
    go install golang.org/x/tools/gopls@latest
    ~~~
- **swag安装（项目集成Swagger）**
    ~~~ commandline  
    go install github.com/swaggo/swag/cmd/swag@latest
    ~~~

## 2、依赖包导入
- 导入依赖包
    ~~~ commandline  
    go mod get ./...
    go mod download #或者
    ~~~

- 清理go.mod和go.sum
    ~~~ commandline  
    go mod tidy
    ~~~

- 将依赖包导入到当前项目目录（防止以后版本冲突问题）
    ~~~ commandline  
    go mod vendor
    ~~~

