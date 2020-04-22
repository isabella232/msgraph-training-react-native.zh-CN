# <a name="how-to-run-the-completed-project"></a>如何运行已完成的项目

## <a name="prerequisites"></a>先决条件

若要在此文件夹中运行已完成的项目，您需要以下各项：

- 至少以下之一：
  - [Android Studio](https://developer.android.com/studio/) **和** [Java 开发工具包](https://jdk.java.net)（在 Android 上运行示例所必需）
  - [Xcode](https://developer.apple.com/xcode/) （在 iOS 上运行示例所必需）
- [Node.js](https://nodejs.org)
- 使用 Outlook.com 上的邮箱的个人 Microsoft 帐户，或者是 Microsoft 工作或学校帐户。

> **注意：** 本教程是使用响应本机 CLI 编写的，其中包含特定的先决条件，具体取决于您的操作系统和目标平台。 有关配置开发计算机的说明，请参阅[响应原生入门](https://facebook.github.io/react-native/docs/getting-started)。 下面列出了用于本教程的版本。 本指南中的步骤可能适用于其他版本，但尚未经过测试。
>
> - 适用于 Android 9.0 SDK 的 android Studio 3.6.2 版本
> - Java 开发工具包版本12.0。2
> - Xcode 版本11。4
> - Node.js 版本12.16。2

如果你没有 Microsoft 帐户，可以使用以下几种方法获取免费帐户：

- 你可以[注册新的个人 Microsoft 帐户](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1)。
- 你可以[注册 office 365 开发人员计划](https://developer.microsoft.com/office/dev-program)以获取免费的 office 365 订阅。

## <a name="register-an-application-with-the-azure-active-directory-admin-center"></a>将应用程序注册到 Azure Active Directory 管理中心

1. 打开浏览器，并转到 [Azure Active Directory 管理中心](https://aad.portal.azure.com)。然后，使用**个人帐户**（亦称为“Microsoft 帐户”）或**工作或学校帐户**登录。

1. 选择左侧导航栏中的“**Azure Active Directory**”，再选择“**管理**”下的“**应用注册**”。

    ![应用注册的屏幕截图 ](/tutorial/images/aad-portal-app-registrations.png)

1. 选择“新注册”****。 在“注册应用”**** 页上，按如下方式设置值。

    - 将“名称”**** 设置为“`React Native Graph Tutorial`”。
    - 将“受支持的帐户类型”**** 设置为“任何组织目录中的帐户和个人 Microsoft 帐户”****。
    - 在 "**重定向 URI**" 下，将下拉列表更改为 "**公用客户端（移动 & 桌面）**"，并将值设置为`graph-tutorial://react-native-auth`。

    !["注册应用程序" 页的屏幕截图](/tutorial/images/aad-register-an-app.png)

1. 选择 "**注册**"。 在 "**响应本机图形教程**" 页上，复制**应用程序（客户端） ID**的值并保存它，下一步将需要它。

    ![新应用注册的应用程序 ID 的屏幕截图](/tutorial/images/aad-application-id.png)

1. 在 "**管理**" 下，选择 "**身份验证**"。 在 "**重定向 uri** " 页上，使用 URI `urn:ietf:wg:oauth:2.0:oob`添加另一个类型为 "**公用客户端（移动 & 桌面）**" 的重定向 uri。 选择“**保存**”。

    !["重定向 Uri" 页的屏幕截图](/tutorial/images/aad-redirect-uris.png)

## <a name="configure-the-sample"></a>配置示例

1. 将**GraphTutorial/auth/AuthConfig 示例**文件重命名为**AuthConfig**。
1. 编辑**AuthConfig**文件并进行以下更改。
    1. 将`YOUR_APP_ID_HERE`替换为你从应用注册门户获取的**应用程序 Id** 。

1. 在命令行界面（CLI）中，导航到**GraphTutorial**目录并运行以下命令以安装要求。

    ```Shell
    npm install
    ```

1. 在命令行界面（CLI）中，导航到**GraphTutorial/ios**目录并运行以下命令以安装要求。

    ```Shell
    pod install
    ```

## <a name="run-the-sample"></a>运行示例

### <a name="run-on-ios-simulator"></a>在 iOS 模拟器上运行

在 CLI 中运行以下命令，以在 iOS 模拟器中启动应用程序。

```Shell
react-native run-ios
```

### <a name="run-on-android-emulator"></a>在 Android 模拟器上运行

启动和 Android 仿真程序实例，并在 CLI 中运行以下命令，以在 Android 模拟器中启动应用程序。

```Shell
react-native run-android
```
