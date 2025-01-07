# Contributing to Free ChatGPT Mirrors / 如何为免费 ChatGPT 镜像站点仓库做贡献

Thank you for your interest in contributing to the Free ChatGPT Mirrors project! We welcome contributions from everyone. / 感谢您有兴趣为免费 ChatGPT 镜像站点项目做出贡献！ 我们欢迎每个人的贡献。

This document outlines the guidelines for contributing to this repository. Please take a moment to review it before submitting your contributions. / 本文档概述了为该仓库做出贡献的准则。 在提交您的贡献之前，请花点时间查看一下。

## Ways to Contribute / 贡献方式

There are many ways you can contribute to this project, including: / 您可以通过多种方式为本项目做出贡献，包括：

*   **Adding new mirror sites:**  If you know of a free ChatGPT mirror site that is not on the list, please submit a pull request to add it. / **添加新的镜像站点：** 如果您知道列表中没有的免费 ChatGPT 镜像站点，请提交拉取请求 (pull request) 以添加它。
*   **Updating existing site information:** If you find any information about a site that is outdated or incorrect, please submit a pull request to update it. / **更新现有站点信息：** 如果您发现某个站点的信息已过时或不正确，请提交拉取请求进行更新。
*   **Fixing typos or grammatical errors:** If you find any typos or grammatical errors in the README or other documentation, please submit a pull request to fix them. / **修复拼写或语法错误：** 如果您在 README 或其他文档中发现任何拼写或语法错误，请提交拉取请求来修复它们。
*   **Improving the documentation:**  If you have any suggestions for improving the documentation, please open an issue or submit a pull request. / **改进文档：** 如果您对改进文档有任何建议，请提出问题 (issue) 或提交拉取请求。
*   **Reporting bugs or issues:** If you find any bugs or issues with the project, please report them by opening an issue. / **报告错误或问题：** 如果您发现项目的任何错误或问题，请通过提出问题来报告它们。

## Guidelines for Adding New Mirror Sites / 添加新镜像站点的准则

When adding a new mirror site, please ensure that it meets the following criteria: / 添加新镜像站点时，请确保其满足以下标准：

*   **Free to use:** The site must be free to use for basic functionalities, at least for a trial period or with certain limitations. / **免费使用：** 该站点必须可以免费使用基本功能，至少在试用期内或有一定限制。
*   **Provides access to a ChatGPT-like model:** The site should provide access to a model similar to ChatGPT, such as GPT-3.5, GPT-4, or other large language models. / **提供对类似 ChatGPT 模型的访问：** 该站点应提供对类似 ChatGPT 的模型的访问，例如 GPT-3.5、GPT-4 或其他大型语言模型。
*   **Functional and stable:** The site should be functional and relatively stable. / **功能正常且相对稳定：** 该站点应功能正常且相对稳定。
*   **No malicious content:** The site must not contain any malicious content or engage in any harmful activities. / **无恶意内容：** 该网站不得包含任何恶意内容或从事任何有害活动。

## How to Submit a Pull Request / 如何提交拉取请求 (Pull Request)

1. **Fork the repository:** Click the "Fork" button in the top right corner of the repository page to create a copy of the repository in your own GitHub account. / **派生 (Fork) 仓库：** 单击仓库页面右上角的“Fork”按钮，在您自己的 GitHub 帐户中创建该仓库的副本。
2. **Clone the forked repository to your local machine:** / **将派生的仓库克隆到您的本地机器：**
    ```
    git clone https://github.com/yangzengye/ChatGPT-Free-Sites.git
    ```
    (Replace `yangzengye` with your GitHub username if you fork to your own account.) / (如果您派生到自己的帐户，请将 `yangzengye` 替换为您的 GitHub 用户名。)
3. **Create a new branch:** / **创建一个新分支：**
    ```
    git checkout -b add-new-site
    ```
    (You can use a different branch name, such as `update-site-info` or `fix-typo`.) / (您可以使用不同的分支名称，例如 `update-site-info` 或 `fix-typo`。)
4. **Make your changes:** Add the new site to the `data.json` file. / **进行更改：** 将新站点添加到 `data.json` 文件中。
5. **Commit your changes:** / **提交您的更改：**
    ```
    git add .
    git commit -m "Add [Site Name] mirror site"
    ```
    (Use a descriptive commit message.) / (使用描述性的提交消息。)
6. **Push your changes to your forked repository:** / **将您的更改推送到您派生的仓库：**
    ```
    git push origin add-new-site
    ```
7. **Open a pull request:** Go to the original repository on GitHub and click the "New pull request" button. Choose your forked repository and branch, then click "Create pull request". / **打开一个拉取请求：** 转到 GitHub 上的原始仓库，然后单击“New pull request”按钮。 选择您派生的仓库和分支，然后单击“Create pull request”。
8. **Describe your changes:** In the pull request description, please clearly explain the changes you have made. / **描述您的更改：** 在拉取请求描述中，请清楚地解释您所做的更改。

## Data Format in `data.json`

The mirror site data is stored in the `data.json` file. Each mirror site is represented as a JSON object with the following fields: / 镜像站点数据存储在 `data.json` 文件中。 每个镜像站点都表示为一个具有以下字段的 JSON 对象：

```json
{
  "id": 1,
  "Icon": "https://s3.xxx.xx/1/1fbbd020ff3e1cd8175ac5977712f9b3.webp",
  "Name": "AItianhu",
  "Description_CN": "无限制的GPT-3.5 服务",
  "Description_EN": "Unlimited GPT-3.5 service",
  "Tags": "",
  "Link": "https://chat10.aiyunos.top"
}
```

*   `id`: A unique numerical ID for the site. / 站点的唯一数字 ID。
*   `Icon`: URL to the site's favicon. / 站点图标的 URL。
*   `Name`: The name of the mirror site. / 镜像站点的名称。
*   `Description_CN`: A brief description of the site in Chinese. / 站点简要中文描述
*   `Description_EN`: A brief description of the site in English. / 站点简要英文描述
*   `Tags`: Tags for the site (can be an empty string). / 站点的标签（可以为空字符串）。
*   `Link`: The URL of the mirror site. / 镜像站点的 URL。

**Please keep the `id` in sequence and do not modify or reuse the `id` of other sites when adding or updating the data.** / **在添加或者更新数据时，请保持 `id` 连续，请勿修改或重复使用其他网站的 `id`。**

## Code Style / 代码风格

There might be no actual source in this project, but for consistency, we use: / 此项目可能没有实际的源代码, 但为了保持一致性，我们使用:

*   Markdown for documentation. / Markdown 格式编写文档。
*   JSON for data storage. / JSON 格式存储数据。

## Contact / 联系方式

If you have any questions, please feel free to open an issue or contact **yangzengye** at **zengyeyang8@gmail.com**. / 如果您有任何问题，请随时提出问题或通过 **zengyeyang8@gmail.com** 与 **yangzengye** 联系。

Thank you for your contributions! / 感谢您的贡献！
