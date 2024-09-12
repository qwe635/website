---
标题：本地源
titleTemplate：参考线
描述：适用于希望下载和组织自己的媒体的用户。
---

#本地源

如果你喜欢下载和组织你的媒体，那么你想知道如何管理你自己的系列在Tachiyomi。

**警告
本页将探索一些高级功能。
:::

##创建本地序列

1.在您指定为存储位置的位置(例如，`/Tachiyomi/`)，应该有一个`当地的`文件夹。将结构正确的系列放入其中(例如`/Tachiyomi/local/`).

    >如果在文件夹中添加系列，建议添加名为`.nomedia`复制到本地文件夹，以便图像不会显示在画廊中。

1.现在，您应该能够访问<NAV到="来源">在……下面**本地源**.

如果您添加了更多章节，则必须手动刷新章节列表(通过下拉该列表)。

支持的章节格式是包含图片的文件夹(例如`.jpg`,`.png`等)或归档文件(`拉链`/`CBZ`,`RAR`/`CBR`，和`EPUB`).
但希望在目录和`拉链`/`CBZ`.

请注意，单个文件夹或归档文件被视为单个章节。例如，Tachiyomi不会自动拆分`EPUB`在应用程序中包含多个章节的文件。

###文件夹结构

Tachiyomi需要特定的文件夹结构才能正确处理本地序列。
本地序列将从`当地的`文件夹。
每个系列必须具有`系列`文件夹和`章节`文件夹。
然后图像将进入章节文件夹。
有关归档文件的详细信息，请参阅下面的内容。
您可以参考以下示例：

*信息示例
<div班级="树">
  <UL>
    <IMGsrc="/img/folder.svg" alt="文件夹" 班级="树图标图标文件夹">
    <跨度班级="文件夹根">[您的存储位置]/本地</跨度>
    <锂>
      <IMGsrc="/img/folder.svg" alt="文件夹" 班级="树图标图标文件夹">
      <跨度班级="文件夹主">[系列标题]</跨度>
      <ul>
        <li>
          <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
          <span class="file jpg">cover<span class="file-extension">.jpg</span></span>
        </li>
        <li>
          <img src="/img/folder.svg" alt="Folder" class="tree-icon icon-folder">
          <span class="folder">chapter_1</span>
          <ul>
            <li><span class="file">image_1<span class="file-extension">.ext</span></span></li>
            <li><span class="file">image_n<span class="file-extension">.ext</span></span></li>
          </ul>
        </li>
        <li>
          <img src="/img/folder.svg" alt="Folder" class="tree-icon icon-folder">
          <span class="folder">chapter_2</span>
          <ul>
            <li><span class="file">image_1<span class="file-extension">.ext</span></span></li>
            <li><span class="file">image_n<span class="file-extension">.ext</span></span></li>
          </ul>
        </li>
        <li>
          <img src="/img/folder.svg" alt="Folder" class="tree-icon icon-folder">
          <span class="folder">chapter_n</span>
          <ul>
            <li><span class="file">image_1<span class="file-extension">.ext</span></span></li>
            <li><span class="file">image_n<span class="file-extension">.ext</span></span></li>
          </ul>
        </li>
      </ul>
    </li>
  </ul>
</div>
:::

Tachiyomi will see three chapters in a single series.
The path to the folder with images must contain both the series title and the chapter name (as seen above).

### Archive files

Archive files such as `ZIP`/`CBZ` are supported but the folder structure inside is not.
Any folders inside the archive file are ignored.
You must place the archive inside the `Series` folder where the name will become the `Chapter` title.
All images inside the archive regardless of folder structure will become pages for that chapter.

#### Example {#example-archives}

:::tabs
== .ZIP
<div class="tree">
  <ul>
    <img src="/img/folder.svg" alt="Folder" class="tree-icon icon-folder">
    <span class="folder root">[your storage location]]/local</span>
    <li>
      <img src="/img/folder.svg" alt="Folder" class="tree-icon icon-folder">
      <span class="folder main">[the series title]</span>
      <ul>
        <li>
          <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
          <span class="file jpg">cover<span class="file-extension">.jpg</span></span>
        </li>
        <li>
          <img src="/img/zip.svg" alt="Compressed File" class="tree-icon icon-zip">
          <span class="file zip">chapter_1<span class="file-extension">.zip</span></span>
          <ul>
            <li>
              <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
              <span class="file jpg">image_1<span class="file-extension">.jpg</span></span>
            </li>
            <li>
              <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
              <span class="file jpg">image_n<span class="file-extension">.jpg</span></span>
            </li>
          </ul>
        </li>
        <li>
          <img src="/img/zip.svg" alt="Compressed File" class="tree-icon icon-zip">
          <span class="file zip">chapter_2<span class="file-extension">.zip</span></span>
          <ul>
            <li>
              <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
              <span class="file jpg">image_1<span class="file-extension">.jpg</span></span>
            </li>
            <li>
              <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
              <span class="file jpg">image_n<span class="file-extension">.jpg</span></span>
            </li>
          </ul>
        </li>
        <li>
          <img src="/img/zip.svg" alt="Compressed File" class="tree-icon icon-zip">
          <span class="file zip">chapter_n<span class="file-extension">.zip</span></span>
          <ul>
            <li>
              <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
              <span class="file jpg">image_1<span class="file-extension">.jpg</span></span>
            </li>
            <li>
              <img src="/img/jpeg.svg" alt="File" class="tree-icon icon-jpeg">
              <span class="file jpg">image_n<span class="file-extension">.jpg</span></span>
            </li>
          </ul>
        </li>
      </ul>
    </li>
  </ul>
</div>
:::

<style scoped>
  @import "../../../.vitepress/theme/styles/tree.styl"
</style>
