### 交接项目文档
#### 主要项目一览
工程名称|仓库|交接人
--|:--:|--:
2.0信息发布主工程|git@code.aliyun.com:magicmind/projectFrameShow.git|宋
2.0任务发布管理|git@code.aliyun.com:magicmind/mm-module-frameshow.git|宋
2.0设备管理|git@code.aliyun.com:magicmind/mm-module-frame-devices.git|宋
2.0多媒体mmDevice服务|git@code.aliyun.com:magicmind/project-mmDevice.git|宋
广铁头条内容管理|git@code.aliyun.com:gttt/gttt-content-mgt.git|刘
3.0任务管理|git@code.aliyun.com:mshow/backend-module-task-manager.git|宋,孟

#### 目前遗留问题:
>* 崇阳项目,取消紧急通知时,会偶尔有不能取消的
```
>* 处理:后台增加逻辑处理,当对某一台设备发送不成功时,会尝试2s一次重新发送消息,直到成功或者次数达到30次
>* 结果:等待观察
>* 当发现有没能取消时,查看后台管理点击按钮时的http请求情况和http返回的数据,(确认是否真的没发通, 若是,可取消30次限制,修改为一直发送知道成功)
```
