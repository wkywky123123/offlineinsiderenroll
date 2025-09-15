[English](https://github.com/wkywky123123/offlineinsiderenroll/blob/master/readme.md)/简体中文

# 离线注册预览猫猫 

![离线注册预览猫猫截图](https://github.com/wkywky123123/offlineinsiderenroll/assets/89382167/2e36384b-822e-4ade-a942-2aa2a6617f28)

## 关于猫猫

离线注册预览猫猫是一个简单的Windows命令提示符脚本，用于给没有登录Microsoft账号或不满足预览体验计划硬件要求要求的用户加入Windows的预览体验计划。

猫猫仅兼容Windows11或Windows10版本1809及更高版本。

## 食用方法

猫猫需要管理权限才能运行。主人可以右键单击猫猫> `以管理员身份运行`

### 安装和配置更改

猫猫会提供***Windows预览体检计划***频道的选择。 要进行选择，请按与主人选择的选项相对应的字母，然后按 Enter。

如果计算机未注册到预览体验计划，系统将提示你重新启动计算机以启用 `Microsoft外部测试版签名`

**注意**：Windows 预览体验计划要求将遥测设置为“发送可选诊断数据”。 将计算机注册到Windows预览体验计划后，请确保诊断数据收集设置设置为“发送可选诊断数据”。如果没有，某些版本可能不会在Windows更新中提供正确的诊断设置。 `Insider Preview`

可以验证或修改诊断设置，如下所示：

***Windows 11:*** `设置` > `隐私和安全` > `诊断和反馈`

***Windows 10:*** `设置` > `隐私` > `诊断和反馈`

### 将 Windows 预览体验计划还原为默认选项

要将 `Windows预览体验计划` 恢复为默认设置，只需在猫猫中选择 `退出所有已经加入的频道` 主人会收到提示，计算机需要重新启动，因为此选项将禁用 `Microsoft 外部测试版签名` 。

## 猫猫是怎么工作的？
猫猫利用了未公开的 `TestFlags` 注册表值。
如果这个值被设置为 `0x20` ，所有对在线 *Windows Insider* 服务的访问都会被禁用。因此，主人可以设置自己的 *Windows Insider Preview* 配置，而不会受到服务联系的覆盖。由于 `Windows Update` 不会检查机器是否真的注册了该程序，主人只需要在注册表中设置正确的值，就会收到 *Insider Preview* 构建的推送。

## 许可证

本项目已获得 MIT 许可证许可。有关详细信息，主人可以参阅。 `LICENSE`
