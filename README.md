# 吃谷小管家

二次元谷子购买记录管理工具，支持图片上传、团名分类、状态追踪、统计图表和 LeanCloud 云端同步。

## 在线体验

👉 [https://lilo-bai.github.io/chigu-manager](https://lilo-bai.github.io/chigu-manager)

## 功能

- **卡片管理**：上传图片、记录谷名/价格/团名/状态/囤货 DDL/备注/记录时间
- **团名看板**：按团名切换 Tab，显示累计金额和状态分布
- **统计图表**：月吃谷/月交肾/食量/肾款，点击展开折线图
- **云端同步**：对接 LeanCloud，跨设备数据不丢失
- **头像个签**：我的页面支持上传头像和编辑个性签名
- **数据备份**：JSON 导入导出

## 开启云端同步

1. 前往 [leancloud.cn](https://leancloud.cn) 注册账号
2. 创建新应用
3. 进入「应用设置」→「应用凭证」，复制 **App ID**、**App Key**
4. 国内版需：「应用设置」→「域名绑定」→ 绑定自定义 API 域名
5. 在应用「我的」→「云端同步」→「配置云端」，填入上述信息
6. 注册/登录账号，即可跨设备同步

## 本地开发

```bash
git clone https://github.com/lilo-bai/chigu-manager.git
cd chigu-manager
# 直接用浏览器打开 index.html 即可
```

## 技术栈

- HTML + CSS + JavaScript（单页应用）
- Chart.js 图表
- LeanCloud 数据存储
- GitHub Pages 部署

## 状态含义

| 状态 | emoji | 说明 |
|------|-------|------|
| 未到货 | 💨 | 已下单，等待到货 |
| 已散 | 🏳️ | 团已解散 |
| 已到货 | 🍽️ | 谷子已到团长处 |
| 已排发 | 🍨 | 已安排发货 |
