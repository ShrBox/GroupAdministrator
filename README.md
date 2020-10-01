# GroupAdministrator

![Java CI with Gradle](https://github.com/ShrBox/GroupAdministrator/workflows/Java%20CI%20with%20Gradle/badge.svg)  
简单的mirai机器人群管插件  
目前仅支持Mirai-console 0.5.2  
Notice：更新0.1.5版本后`config.yml`中的`key_words`项需要移动至`key_words.yml`

# Download

[Github Actions](https://github.com/ShrBox/GroupAdministrator/actions)

## Configuration files

- `config.yml`：配置文件  
`accept_word`：如果加群申请内包含该list中的词（大小写不敏感），将会自动同意该申请  
`EnableLeaveMessage`：是否在成员退群时发送群内消息  
`EnableAuditRequests`：是否打开自动审核功能（Notice：打开自动审核后会导致[Verification](https://github.com/ShrBox/Verification) 功能失效）
- `key_words.yml`：禁言词列表  
`key_word`：如果群成员的消息内包含该list中的词，该成员的消息将会被撤回，并且将禁言该成员600秒  

## Command

`/gareload`：重载config.yml
