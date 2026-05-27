# 吃谷小管家

二次元谷子购买记录管理工具，支持图片上传、团名分类、状态追踪、统计图表和 CloudBase 云端同步。

## 在线体验

👉 [https://lilo-bai.github.io/chigu-manager](https://lilo-bai.github.io/chigu-manager)

## 功能

- **卡片管理**：上传图片、记录谷名/价格/团名/状态/囤货 DDL/备注/记录时间
- **团名看板**：按团名切换 Tab，显示累计金额和状态分布
- **统计图表**：月吃谷/月交肾/食量/肾款，点击展开折线图
- **云端同步**：对接腾讯云 CloudBase，跨设备数据不丢失
- **头像个签**：我的页面支持上传头像和编辑个性签名
- **数据备份**：JSON 导入导出

## 开启云端同步

1. 前往 [腾讯云 CloudBase 控制台](https://console.cloud.tencent.com/tcb) 创建环境
2. 在「环境」页面获取 **环境 ID**（EnvID）
3. 到「数据库」页面创建集合 `cards`
4. 设置数据库权限为「所有用户可读，仅创建者可写」（或更开放的权限以支持同步码模式）
5. 在应用「我的」→「云端同步」→「配置云端」，填入环境 ID
6. 设置同步码，换设备输入相同同步码即可同步数据

## 本地开发

```bash
git clone https://github.com/lilo-bai/chigu-manager.git
cd chigu-manager
# 直接用浏览器打开 index.html 即可
```

## 技术栈

- HTML + CSS + JavaScript（单页应用）
- Chart.js 图表
- 腾讯云 CloudBase（数据库 + 文件存储）
- GitHub Pages 部署

## 状态含义

| 状态 | emoji | 说明 |
|------|-------|------|
| 未到货 | 💨 | 已下单，等待到货 |
| 已散 | 🏳️ | 团已解散 |
| 已到货 | 🍽️ | 谷子已到团长处 |
| 已排发 | 🍨 | 已安排发货 |
