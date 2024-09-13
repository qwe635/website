---
标题：入门
titleTemplate：参考线
说明：帮助您设置Tachiyomi的基本信息。
---

<脚本设置 朗="ts">
进口 {数据作为 释放 } 从……起 "@theme/data/release.data"
</脚本>

#入门

帮助您设置Tachiyomi的基本信息。

##安装指南

###正在下载Tachiyomi

1.访问我们的[下载](/news/2024-01-13-再见)获取最新版本的页面**立见**.
2.下载完成后，打开`.apk`文件。
3.继续安装过程。

###添加源

一次**立见**已安装在您的设备上，您可以从各种来源读取您自己的内容：

：：：：选项卡
==本地源
读取设备上本地存储的内容。

请参阅[本地源指南](/docs/指南/本地来源/)以获取指示。
==外部存储库
外部存储库将其他源添加到**立见**。您可以通过以下方式添加外部存储库：<NAV到="浏览">和攻丝**扩展回购**.

在此之后，您可以通过输入URL结尾为`index.min.json`。有一小部分扩展可用[在这里](/extensions/).

*危险警告
Tachiyomi不会为任何非官方存储库提供资源。请注意，任何第三方存储库或扩展将拥有对应用程序的完全访问权限，并且可能包含恶意软件。
:::

添加存储库后，请转到<NAV到="扩展名">并刷新扩展列表。

您现在可以点击扩展名旁边的下载按钮来安装扩展名。

>您可能需要[启用第三方安装](/docs/faq/browse/extensions#启用-第三方-安装).

*提示官方资料库
Tachiyomi有一个官方的扩展库，您可以使用**添加存储库**上的按钮[扩展](/extensions/)页，或在下面手动复制url。
> `https://raw.githubusercontent.com/tachiyomiorg/extensions/repo/index.min.json`
:::
== Manual extensions
Extensions can be manually installed through `.apk` files.

::: danger Caution
Tachiyomi will not provide resources for any unofficial extensions. Beware that any third-party repositories or extensions will have full access to the app and may contain malware.
:::
::::

### Adding series to your library

After installing the desired extension, you'll find it in the **Sources** tab.

Here's how you can add series to your library:

1. Select the source you'd like to browse.
1. You can use the **Popular**/**Latest** listings to browse, or you can search for the series name.
1. Once you've found the series that you want to add, tap on it for more details.
1. Press the "**Add to library**" button, and the series will be added to your Library, ready to be read!

## Additional setup

### Series search options

If you want to search for series across all your sources, you can use the Global Search feature.

Follow these steps:

1. Go to the "**Browse**" section.
1. Ensure you're on the "**Sources**" tab located at the top-right corner.
1. Use the Search icon in the toolbar to find series from all available sources.

### Trouble finding a specific series?

If you encounter difficulties while searching for a specific series, consider the following points:

* Double-check your spelling and try again, as some sources might use **Japanese romanized** titles instead of **English** ones.
  > Example: **Boku no Hero Academia** instead of **My Hero Academia**.

* Some sources may use different spellings or wordings for titles.
  > Example: **Bungo Stray Dogs** instead of **Bungou Stray Dogs**

  > Example: **3-gatsu no Lion** instead of **Sangatsu no Lion**.
