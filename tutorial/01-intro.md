<!-- markdownlint-disable MD002 MD041 -->

本教程向您介绍如何构建使用 Microsoft Graph API 来检索用户的日历信息的响应本机应用程序。

> [!TIP]
> 如果您只想下载已完成的教程，可以下载或克隆[GitHub 存储库](https://github.com/microsoftgraph/msgraph-training-react-native)。

## <a name="prerequisites"></a>先决条件

在开始本教程之前，您应在开发计算机上安装以下程序。

- 至少以下之一：
  - [Android Studio](https://developer.android.com/studio/) **和** [Java 开发工具包](https://jdk.java.net)（在 Android 上运行示例所必需）
  - [Xcode](https://developer.apple.com/xcode/) （在 iOS 上运行示例所必需）
- [Node.js](https://nodejs.org)

您还应具有一个个人的 Microsoft 帐户，其中包含 Outlook.com 上的邮箱，或 Microsoft 工作或学校帐户。 如果你没有 Microsoft 帐户，可以使用以下几种方法获取免费帐户：

- 你可以[注册新的个人 Microsoft 帐户](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1)。
- 你可以[注册 office 365 开发人员计划](https://developer.microsoft.com/office/dev-program)以获取免费的 office 365 订阅。

> [!NOTE]
> 本教程是使用响应本机 CLI 编写的，其中包含特定的先决条件，具体取决于您的操作系统和目标平台。 有关配置开发计算机的说明，请参阅[响应原生入门](https://reactnative.dev/docs/environment-setup)。 下面列出了用于本教程的版本。 本指南中的步骤可能适用于其他版本，但尚未经过测试。
>
> - 适用于 Android 9.0 SDK 的 android Studio 3.6.2 版本
> - Java 开发工具包版本12.0。2
> - Xcode 版本11。4
> - Node.js 版本12.16。2

## <a name="feedback"></a>反馈

请在[GitHub 存储库](https://github.com/microsoftgraph/msgraph-training-react-native)中提供有关本教程的任何反馈。
