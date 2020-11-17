# CWIKIUS  Docker 文档和手册

欢迎来到 CWIKIUS Docker 文档和手册的空间

本文档的编译发布版本访问地址：[docker-docs.ossez.com](https://docker-docs.ossez.com)

CWIKIUS 的有关 Docker 相关文档：[https://www.cwiki.us/display/DockerZH/Docker](https://www.cwiki.us/display/DockerZH/Docker)

GitHub 上有关 CWIKIUS Docker 的项目的源代码文件：[https://github.com/cwiki-us-docs/docker-docs](https://github.com/cwiki-us-docs/docker-docs)

如果您有兴趣参与我们的小组和项目，请使用下面的联系方式和我们联系：

| 联系方式名称  | 联系方式  |
|---|---|
| 电子邮件  | [service@ossez.com](mailto:service@ossez.com)  |
| QQ 或微信  | 103899765  |
| QQ 交流群 Spring | 15186112 |
| 社区论坛 | [https://www.ossez.com/c/Toolkit-Algorithm-Computer-Science/system-and-container/25](https://www.ossez.com/c/Toolkit-Algorithm-Computer-Science/system-and-container/25) |

## 微信及公众平台
我们建议您通过社区论坛来和我们进行沟通，请关注我们的微信公众号。

![](https://cdn.ossez.com/img/cwikius/cwikius-qr-wechat-search-w400.png)

## CWIKIUS 文档和手册快速导航
有关相关文档和我们参考过的一些内容的快速导航。

| 网站地址  | 网站链接  |
|---|---|
| CWIKIUS Docker Docs 在线文档  | https://docker-docs.ossez.com |
| CWIKI.US 空间  | https://www.cwiki.us/display/DockerZH/Docker  |
| Docker 官方文档 | https://docs.docker.com/ |
| chinese_docker | https://github.com/widuu/chinese_docker |
| daocloud.io | https://guide.daocloud.io/#all-updates |

欢迎来到 Docker 文档的代码仓库。本代码仓库是文档 https://docs.docker.com 的源代码。

如果你发现这个文档有任何问题，Docker 官方欢迎你来创建 合并请求（Pull Requests）。Docker 的文档是完全开源的，Docker 官方也非常感谢社区对 Docker 的贡献。

## 提供反馈

Docker 的官方和 CWIKIUS 都非常欢迎您对我们的内容进行反馈，并且我们将这个提供反馈的方法进行了调整，以便于更好的进行访问和提交。你可以对页面进行编辑或者针对 https://docs.docker.com 上每一个页面的右上角提供的链接来对内容进行编辑和提交合并请求。

你也可以对每一个页面来进行评分，评分的链接在页面的页脚。

**本仓库只针对文档的内容进行修改。** 如果你考虑对文档进行修改的话，在提交 PR 之前你应该先考虑下这个问题应该是和文档相关的，比如说文档描述的不清楚，文档出现了错误，或者在文档让用户非常困惑等。

* 如果你在使用 Docker 的时候遇到了问题，请访问 https://forums.docker.com 论坛中的内容。
* 如果针对 Docker 的新功能和特性有什么更好的建议或者你找到了 Docker 的一个 bug，请使用 Docker 的代码仓库来提交你的问题。

## 贡献

我们非常重视你对文档的贡献，我们也希望能够尽可能的在文档仓库中间的的工作。

在你决定对文档进行贡献的时候，你需要首先确定你希望工作的分支。如果你在这个上面有什么困惑的话，你只需要向我们提问即可，官方和我们都会尽可能的帮助你。

如果官方的开放人员或者其他人发现了你可能提交了错误的分支，将会有人提醒你的，这个时候你只需要 rebase 你的工作就可以了。

> **Note**: 希望对 Docker 的开发贡献你自己的力量？请参考下面文档的内容：[Contribution guidelines](CONTRIBUTING.md)。

### 不需要在这里编辑的文件

文件或者目录列在为 

[`.NOT_EDITED_HERE.yaml`](.NOT_EDITED_HERE.yaml) 

关键字的路径被其他仓库使用的是不应该进行编辑的。

对上面字符串进行编辑后提交的 PR 请求会被驳回（rejected），请确定你编辑的仓库中的文件和路径是正确的。

### 文档改善计划概述

合并请求（PR）应该是针对 `master` 分支提出的，这个内容包括有：

* 不针对新特性的概念性的内容和基于任务的信息
* 重新格式化或者重写部分内容
* 文档错误的修改
* 拼写或者语法错误

> 你是否享受创建一些图形呢？好看漂亮的图形和设计是一个好文档的关键，我们尤其欢迎您在这个方面的贡献和帮助。

## GitHub 提交 合并请求（PR） 之前的预存（staging ）

针对提交到 `master` 分支的每一次合并请求，一个针对站点使用 Netlify 的预存 staging 将会被创建。

如果站点被重构创建，将会看到 **deploy/netlify — Deploy preview ready**** 文字。

否则的话，你将会看到一个错误信息，单击 **Details** 来查看暂存的站点或者阻止站点重构的错误。重新查看暂存的站点来确定是不是你提交的内容导致的错误。

在 PR 合并到 master 分支之前，其他的项目相关人员同时也会查看暂存的站点。通过这个选项，我们来保护 https://docs.docker.com 站点不会有错误。

## 在本地构建和查看文档

On your local machine, clone this repo:

```bash
git clone --recursive https://github.com/docker/docker.github.io.git
cd docker.github.io
```

Then build and run the documentation with [Docker Compose](https://docs.docker.com/compose/)

```bash
docker-compose up -d --build
```

> Docker Compose is included with [Docker Desktop](https://docs.docker.com/desktop/).
> If you don't have Docker Compose installed, [follow these installation instructions](https://docs.docker.com/compose/install/).

Once the container is built and running, visit [http://localhost:4000](http://localhost:4000)
in your web browser to view the docs.

To rebuild the docs after you made changes, run the `docker-compose up` command
again. This rebuilds the documentation, and updates the container with your changes:

```bash
docker-compose up -d --build
```

Once the container is built and running, visit [http://localhost:4000](http://localhost:4000)
in your web browser to view the docs.


To stop the staging container, use the `docker-compose down` command:

```bash
docker-compose down
```

### Build the docs with deployment features enabled

The default configuration for local builds of the documentation disables some
features to allow for a shorter build-time. The following options differ between
local builds, and builds that are deployed to docs.docker.com:

- search auto-completion, and generation of `js/metadata.json`
- google analytics
- page ratings
- `sitemap.xml` generation
- minification of stylesheets (css/style.css)
- adjusting "edit this page" links for content in other repositories

If you want to contribute in these areas, you can perform a "production" build
locally.

To preview the documentation with deployment features enabled, you need to set the
`JEKYLL_ENV` environment variable when building the documentation;

```bash
JEKYLL_ENV=production docker-compose up --build
```

Once the container is built and running, visit [http://localhost:4000](http://localhost:4000)
in your web browser to view the docs.

To rebuild the docs after you make changes, repeat the steps above.

<!--
TODO re-enable auto-builds, or push master builds to Docker hub
## Read these docs offline

To read the docs offline, you can use either a standalone container or a swarm service.
To see all available tags, go to [Docker Hub](https://docs.docker.com/docker-hub/).

The following examples use the `latest` tag:

- Run a single container:

  ```bash
  docker run  -it -p 4000:4000 docs/docker.github.io:latest
  ```

- Run a swarm service:

  ```bash
  docker service create -p 4000:4000 --name localdocs --replicas 1 docs/docker.github.io:latest
  ```

  This example uses only a single replica, but you could run as many replicas as you'd like.

Either way, you can now access the docs at port 4000 on your Docker host.
-->

## 重要的文件

- `/_data/toc.yaml` defines the left-hand navigation for the docs
- `/js/docs.js` defines most of the docs-specific JS such as TOC generation and menu syncing
- `/css/style.scss` defines the docs-specific style rules
- `/_layouts/docs.html` is the HTML template file, which defines the header and footer, and includes all the JS/CSS that serves the docs content

## Relative linking for GitHub viewing

Feel free to link to `../foo.md` so that the docs are readable in GitHub, but keep in mind that Jekyll templating notation
`{% such as this %}` will render in raw text and not be processed. In general it's best to assume the docs are being read
directly on [https://docs.docker.com/](https://docs.docker.com/).

### Testing changes and practical guidance

If you want to test a style change, or if you want to see how to achieve a
particular outcome with Markdown, Bootstrap, JQuery, or something else, have
a look at `test.md` (which renders in the site at `/test/`).

### Per-page front-matter

The front-matter of a given page is in a section at the top of the Markdown
file that starts and ends with three hyphens. It includes YAML content. The
following keys are supported. The title, description, and keywords are required.

| Key                    | Required  | Description                             |
|------------------------|-----------|-----------------------------------------|
| title                  | yes       | The page title. This is added to the HTML output as a `<h1>` level header. |
| description            | yes       | A sentence that describes the page contents. This is added to the HTML metadata. |
| keywords               | yes       | A comma-separated list of keywords. These are added to the HTML metadata. |
| redirect_from          | no        | A YAML list of pages which should redirect to THIS page. At build time, each page listed here is created as a HTML stub containing a 302 redirect to this page. |
| notoc                  | no        | Either `true` or `false`. If `true`, no in-page TOC is generated for the HTML output of this page. Defaults to `false`. Appropriate for some landing pages that have no in-page headings.|
| toc_min                | no        | Ignored if `notoc` is set to `true`. The minimum heading level included in the in-page TOC. Defaults to `2`, to show `<h2>` headings as the minimum. |
| toc_max                | no        | Ignored if `notoc` is set to `false`. The maximum heading level included in the in-page TOC. Defaults to `3`, to show `<h3>` headings. Set to the same as `toc_min` to only show `toc_min` level of headings. |
| no_ratings             | no        | Either `true` or `false`. Set to `true` to disable the page-ratings applet for this page. Defaults to `false`. |
| skip_read_time         | no        | Set to `true` to disable the 'Estimated reading time' banner for this page. |
| sitemap                | no        | Exclude the page from indexing by search engines. When set to `false`, the page is excluded from `sitemap.xml`, and a `<meta name="robots" content="noindex"/>` header is added to the page. |

The following is an example of valid (but contrived) page metadata. The order of
the metadata elements in the front-matter is not important.

```liquid
---
description: Instructions for installing Docker on Ubuntu
keywords: requirements, apt, installation, ubuntu, install, uninstall, upgrade, update
redirect_from:
- /engine/installation/ubuntulinux/
- /installation/ubuntulinux/
- /engine/installation/linux/ubuntulinux/
title: Get Docker for Ubuntu
toc_min: 1
toc_max: 6
skip_read_time: true
no_ratings: true
---
```

### Creating tabs

The use of tabs, as on pages like [https://docs.docker.com/engine/api/](/engine/api/), requires
the use of HTML. The tabs use Bootstrap CSS/JS, so refer to those docs for more
advanced usage. For a basic horizontal tab set, copy/paste starting from this
code and implement from there. Keep an eye on those `href="#id"` and `id="id"`
references as you rename, add, and remove tabs.

```html
<ul class="nav nav-tabs">
  <li class="active"><a data-toggle="tab" data-target="#tab1">TAB 1 HEADER</a></li>
  <li><a data-toggle="tab" data-target="#tab2">TAB 2 HEADER</a></li>
</ul>
<div class="tab-content">
  <div id="tab1" class="tab-pane fade in active">TAB 1 CONTENT</div>
  <div id="tab2" class="tab-pane fade">TAB 2 CONTENT</div>
</div>
```

For more info and a few more permutations, see `test.md`.

### Running in-page Javascript

If you need to run custom Javascript within a page, and it depends upon JQuery
or Bootstrap, make sure the `<script>` tags are at the very end of the page,
after all the content. Otherwise the script may try to run before JQuery and
Bootstrap JS are loaded.

> **Note**: In general, this is a bad idea.

### Images

Don't forget to remove images that are no longer used. Keep the images sorted
in the local `images/` directory, with names that naturally group related images
together in alphabetical order. For instance prefer `settings-file-share.png`
and `settings-proxies.png` to `file-share-settings.png` and
`proxies-settings.png`. You may also use numbers, especially in the case of a
sequence, e.g., `run-only-the-images-you-trust-1.svg`
`run-only-the-images-you-trust-2.png` `run-only-the-images-you-trust-3.png`.

When applicable, capture windows rather than rectangular regions. This
eliminates unpleasant background and saves the editors the need to crop.

On Mac, capture windows without shadows. To this end, once you pressed
`Command-Shift-4`, press Option while clicking on the window. To disable
shadows once for all, run:

```bash
$ defaults write com.apple.screencapture disable-shadow -bool TRUE
$ killall SystemUIServer  # restart it.
```

You can restore shadows later with `-bool FALSE`.

In order to keep the Git repository light, _please_ compress the images
(losslessly). On Mac you may use (ImageOptim)[https://imageoptim.com] for
instance. Be sure to compress the images *before* adding them to the
repository, doing it afterwards actually worsens the impact on the Git repo (but
still optimizes the bandwidth during browsing).

## Copyright and license

Copyright 2013-2020 Docker, inc, 文件的发布是基于 Apache 2.0 license 下进行发布。

中文版本的翻译和维护由 CWIKIUS 进行。我们允许在非商业的情况下自由扩散分发，并保留适当的权利。您可以对我们的作品进行演绎，但需要保留版权信息和来源。