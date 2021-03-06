# 更新记录

## 正式版 （即将发布）

1. 稳定性增强

## RC2 （即将发布）

1. 加入Notadd Store （Beta）
2. 数据库读写分离方案
3. 性能优化


## RC （即将发布）

1. 模块与插件安装、更新机制
3. 大量的BUG修复
4. 引入验证码插件，后台默认启用
5. 模块信息注入
6. 支持更多缓存
7. 支持后台管理拓展

## Beta6 fix3 (071127)

1. 合并static 与 public 目录，与 laravel 相同。
2. 修复 mac 下因系统信息显示导致无法登陆后台的BUG
3. 修复 windows 下显示乱码的BUG [@yudan215](https://github.com/yudan215)
4. 移除默认 ECDSA 加密，改为 hash384 


## Beta6 fix2 (071109)

1. 开发者名单展示优化
2. 更全面及精准的系统信息显示
3. more

## Beta6 fix1 (071105)

1. 安装时，Redis 的检测及状态提示更加详细
2. 添加更多的 GraphQL 接口
3. 修复其他 bug

## Beta6 (071030)

1. 默认 GraphQL API
2. 修复安装时数据库地址不能输入 IP 的问题
3. 修复安装时数据库密码不能输入"." 的BUG

## Beta5 fix2 (071017)

1. 添加单元测试代码
2. 添加功能测试代码
3. 重构 JWT 验证机制
4. 修正安装时对数据库及Redis连接、账号和密码的验证
5. 扩展 MIME 类型，使返回的文件头信息正常
6. 优化后台导航栏加载机制
7. 优化后台侧边栏加载机制
8. 修复后台导航栏无法加载模块导航的问题
9. 修复后台侧边栏无法加载自定义页面菜单的问题
10. 修复后台侧边栏无法加载插件菜单的问题
11. 修复后台加载图形无法显示的问题
12. 添加将域名配置写入json文件的功能（statics 目录下的 configuration.json）
13. 重构模块安装流程
14. 重构插件安装流程
15. 重构模块开启/加载逻辑
16. 重构插件开启/加载逻辑
17. 修正配置文件缓存机制

## Beta5 fix1 （170928）

1. 添加底层缓存机制，优化并提升性能（约5倍）
2. 修复安装检测 public 及 pdo_mysql 问题
3. 修复模块和插件加载的问题
4. 修复树莓派下不能正常安装的问题
5. 后台添加 Redis 版本的显示
6. 后台系统信息显示优化
7. 合并后台前端资源文件
8. 修复 js 头部响应为 json 的问题

## Beta5 （170926）

1. 添加拓展机制，暂无后台
2. 完善后台菜单的管理逻辑
3. 主体框架、模块、插件的事件订阅器的自动发现
4. 模块、插件的命令行命令的自动发现
5. 资源（Resource）路由添加对控制器方法名的自定义
6. Monaco 代码编辑器二次加载失败的 Bug
7. 升级前端项目打包工具 Wepack 为版本 3

## Beta4（170913）

1. 新SEO方案
2. 默认使用Redis缓存 
3. 基于Laravel 5.5.3
4. 后台模块排序
5. 修复 模块别名问题

## Beta3 fix1（170904）

1. 后台首页可拖动
2. 全新后台界面和登录界面
3. 修正`statics`目录下部分资源不显示的问题
4. 静态文件发布到`statics`的遗留问题
5. 修复后台分页报错的BUG

## Beta3 （170822）

1. 添加工作流支持
2. 添加多域名支持
3. 添加模块/插件的配置和数据导入/导出
4. 添加模块域名
5. 添加自定义配置页面（前端免编码）
6. 优化后台操作体验
7. 调整服务器框架

## Beta2 fix1 （170527）

1. 增强安装的逻辑处理
2. 移除后台登录二次请求链接的问题
3. 增强了权限架构（四级）
4. 修复后台偶尔不能登录的问题
5. 修复框架层文件缺失问题

## Beta2 （170411）

1. 更新Laravel到5.4（涉及结构调整）
2. 增加用户中心模块。
3. 文章多用户支持（需要安装用户中心模块）
4. 模块、插件的完整卸载安装、启用关闭机制。
5. 新版的安装引导界面。
6. 用户中心消息通知。

## Beta1 fix3 （170305）
1. 文章分类管理移动出错的BUG,目前移动后切换路由。
2. 修复分类名称不能修改的BUG。
3. 一定程度下解决，网络问题下文章重复发布的BUG
4. 页面无法发布问题（开发群 @半缕阳光）
5. 后台增加跳转到首页功能 （开发群 @半缕阳光）
6. 回收站“反选”按钮无法使用的BUG （开发群 @半缕阳光）
7. 草稿箱编辑部分内容，一直增加草稿的BUG（开发群 @半缕阳光）
8. 全站开启关闭按钮无用的BUG。

## Beta1 fix2 （170226）

主要解决上个版本遗留问题，整体体验更好。
1. 插件的开启、关闭、安装、卸载，插件声明相关依赖插件。
2. 模块的开启和关闭 （安装和卸载 在Beta2 中实现）
3. 整体体验的优化。
4. Vue 动态加载重写。
5. 前台SEO收录问题。

## Beta1 fix1 （170220）

1. 修复windows下报错问题 。（开发群 @Sher）
2. 修复postgresql 数据库下 文章发布的BUG。
3. 优化后台提示信息。
4. 修复某些情况更新配置失败的问题.
5. 修复文章和页面没有分类选择的BUG。（开发群 @半缕阳光）
6. 增加文章和页面按分类筛选。


##  Beta1 （170219）

其实这个版本来说，还是相当不完美的版本。以下是已知BUG：

1. 由于Vue单页应用原因，插件无法动态加载。
2. 分类的排序存在很大BUG，目前不建议过多拖动。
3. 前台文章SEO问题，由于SPA单页应用的问题，目前不能被搜索引擎收录。
4. 安装和后台的一些细节提示尚待优化。

由于相对之前版本，底层有改动，故不再列出之前Alpha系列版本。
