# 社区文件共享 Community Files

_试运行 (In Beta)_

**Flutter 社区文件共享平台：**

提供内容同步以及社区教程投稿时需要图片、代码等小文件存储的服务。
通过向本仓库提交 Pull Request，合并之后即可部署到 files.flutter-io.cn，下简称「文件平台」。

**特别说明：**

- 请自行确保文件合法合规，并且个人拥有使用权之后再向文件平台提交
- 仓库文件的数据流向为: GitHub Actions --> 阿里云 OSS 专用 bucket --> 同区域复制 (增/改同步; 全部文件进行同步) -> 阿里云 OSS 生产环境 OSS --> 阿里云 CDN
- 尚未确定文件更新之后 OSS 和 CDN 的数据联动，因此如果有文件更新需求，可首选以更新文件名的方式更新
- - 为了确保数据完整性，我们只设定了增/改同步，因此，在文件平台仓库删除文件后不会影响生产环境的文件，如果希望删除文件或刷新 CDN 缓存，请发 issue 告诉我们

如果有任何问题和建议，欢迎通过 issue 的方式提出，再次谢谢所有愿意为社区贡献的开发者！
