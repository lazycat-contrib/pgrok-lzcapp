# pgrok for LazyCat

上游：https://github.com/pgrok/pgrok

包名：community.lazycat.app.pgrok（前缀来源 default）

Mirror 模式，跟踪镜像稳定 SemVer，目标 linux/amd64；只发布喵喵商店。

安装时必须填写可用的 OIDC 身份提供方与通配隧道域名。管理界面通过 OIDC 登录；TCP 2222 为 SSH 隧道入口，3000 为 HTTP 隧道入口，均需用户自行配置网络可达性和通配 DNS。不提供任意 TCP 端口范围转发。数据库密码自动生成并稳定保存。配置文件按安装参数重建，勿直接编辑运行目录。

public_path / 按用户要求开放，保留上游自身认证。文件操作接入懒猫网盘选择器。图标为上游组织 GitHub 头像。

GitHub Action 默认 dry-run；手动将 dry-run=false 才会正式发布。组织配置 APPSTORE_URL、APPSTORE_TOKEN、可选 PRIVATE_STORE_GROUP_CODES。
