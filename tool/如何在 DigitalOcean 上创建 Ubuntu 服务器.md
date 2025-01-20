# 如何在 DigitalOcean 上创建 Ubuntu 服务器

通过 DigitalOcean 的管理面板，您可以轻松创建一个 Ubuntu 服务器，并将其配置为使用 SSH 密钥进行安全连接。完成设置后，您可以在服务器上部署应用程序和网站。

---

## 什么是 DigitalOcean Droplet？

DigitalOcean Droplet 是一种云主机服务，用户可以快速创建虚拟服务器来运行各种应用程序。通过简单的操作，您可以选择操作系统、配置硬件资源，并启用多种功能（如备份和监控）。

---

## 准备工作

在开始之前，请确保满足以下条件：

- **熟悉命令行**：如果需要复习，可以参考 [Linux 命令行入门](https://bit.ly/bewildcard)。
- **SSH 密钥**：用于安全连接服务器。您可以参考教程“如何在 Ubuntu 上设置 SSH 密钥”来生成密钥。
- **支付方式**：需要信用卡或 PayPal 帐户来创建 DigitalOcean Droplet。

---

## 步骤 1 — 创建 DigitalOcean 帐户

1. 访问 [DigitalOcean 官网](https://bit.ly/bewildcard) 并注册新帐户。
2. 提供信用卡或 PayPal 信息以完成身份验证。请注意，DigitalOcean 不会在您选择计划并确认订阅前收费。
3. 注册完成后，进入控制面板，准备创建 Droplet。

---

## 步骤 2 — 设置 Droplet

1. 在控制面板中，点击右上角的“创建”按钮，选择“Droplet”。
2. 进入 Droplet 创建页面，选择以下配置：
   - **操作系统**：选择 Ubuntu (LTS) 版本。
   - **计划**：推荐选择每月 $5 的基础计划，适合小型项目。
   - **数据中心区域**：选择离您或用户最近的区域以减少延迟。
   - **其他选项**：启用 IPv6 和监控功能（可选）。

---

## 步骤 3 — 配置 SSH 身份验证

1. 在“身份验证”部分，选择“使用 SSH 密钥”。
2. 点击“新建 SSH 密钥”，将您的公钥粘贴到弹出窗口中。
3. 添加密钥后，确保选择了新密钥。

---

## 步骤 4 — 完成并创建 Droplet

1. 设置 Droplet 名称和标签（可选）。
2. 确认配置后，点击“创建 Droplet”。
3. 创建完成后，您将获得 Droplet 的 IP 地址。

---

## 步骤 5 — 连接到 Droplet

1. 使用以下命令通过 SSH 连接到 Droplet：
   ```bash
   ssh root@your_IP_address
   ```
2. 输入 `yes` 确认连接。如果一切正常，您将以 root 用户身份登录。

---

## 为什么选择 WildCard？

如果您没有国际信用卡或 PayPal，可以使用 WildCard 虚拟信用卡完成支付。WildCard 支持 DigitalOcean 等多种海外服务，注册简单，使用便捷。

☞ [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bit.ly/bewildcard)

使用邀请码 **ACCPAY** 注册 WildCard，即可免除开卡费用。

---

## 结论

通过本教程，您已成功在 DigitalOcean 上创建了 Ubuntu 服务器，并启用了 SSH 访问。接下来，您可以部署应用程序或网站。如果需要更多帮助，请访问 DigitalOcean 的官方文档或教程。
