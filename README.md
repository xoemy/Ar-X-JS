
为 JS 平台而生

* * *
* * *


### PaaS 平台用到的变量:
 
* 在 `server.js` 文件的第1、2行修改查询网页的用户名和密码
  | 变量名        | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | WEB_USERNAME | 是 | admin | 网页的用户名 |
  | WEB_PASSWORD | 是 | password | 网页的密码 |

<img width="939" alt="image" src="https://user-images.githubusercontent.com/92626977/221387298-4183a1d6-ae14-45f9-b498-1789a4f7117e.png">

* 在 `entrypoint.sh` 文件的前面 4-12 行修改；访问页面的认证在 `server.js` 文件的第1、2行修改必填
  | 变量名        | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | UUID         | 否 | de04add9-5c68-8bab-950c-08cd5320df18 | 可在线生成 https://www.zxgj.cn/g/uuid |
  | WSPATH       | 否 | argo | 勿以 / 开头，各协议路径为 `/WSPATH-协议`，如 `/argo-vless`,`/argo-vmess`,`/argo-trojan`,`/argo-shadowsocks` |
  | NEZHA_SERVER | 否 |        | 哪吒探针服务端的 IP 或域名 |
  | NEZHA_PORT   | 否 |        | 哪吒探针服务端的端口 |
  | NEZHA_KEY    | 否 |        | 哪吒探针客户端专用 Key |
  | ARGO_AUTH    | 否 |        | Argo 的 Token 或者 json 值，其中 json 可以通过以下网站，在不需绑卡的情况下轻松获取: https://fscarmen.cloudflare.now.cc/ |
  | ARGO_DOMAIN  | 否 |        | Argo 的域名，须与 ARGO_DOMAIN 必需一起填了才能生效 |

<img width="1301" alt="image" src="https://user-images.githubusercontent.com/92626977/226095672-ecbfc8e7-80f3-4821-abb4-df75c4ece483.png">

* 需要应用的 js
  | 命令 | 说明 |
  | ---- |------ |
  | <URL>/list | 查看节点数据 |
  | <URL>/status | 查看后台进程 |
  | <URL>/listen | 查看后台监听端口 |

