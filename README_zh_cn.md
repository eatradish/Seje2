# 寫嘢

![screenshot](screenshot.png)

[Demo](https://eatradish.github.io/Seje2)

## 安装
确保使用 zola init myblog 创建了你的 zola 博客文件夹，然后将 Seje2 克隆到本地 themes 文件下：

```bash
cd themes
git clone https://github.com/eatradish/Seje2
```

之后在 `config.toml` 文件中指定 theme 为 Seje2：

```toml
theme = "Seje2"
```

之后需要你修改 content 的 index 文件 (`content/_index.md`) 来设置在首页中一页能显示多少篇文章：

```toml
paginate_by = 5
```


以及，在你的关于页面 (`about/_index.md`) 中，添加以下行：

```toml
title = "..."

[extra]
year = 2019
month = 11
day = 3
```

## 选项

### 菜单栏
要修改菜单栏的内容，请修改 `config.toml` extra 中 `seje2_menu_links` 的内容，像下面这样:

```toml
seje2_menu_links = [
    {url = "$BASE_URL", name = "Home"},
    {url = "$BASE_URL/categories", name = "Categories"},
    {url = "$BASE_URL/tags", name = "Tags"},
    {url = "https://google.com", name = "Google"},
]
```

这个 BASE_URL 是你在 `config.toml` 中 `base_url` 字段的内容，像 demo 中就是：

```toml
base_url = "https://blog.miraclemilk.me/Seje2"
```

### 文章版权

可以在 `config.toml` 的 `extra` 中修改 `License 字段的内容`，来设置你的文章版权显示:

```toml
license = "@ 宇宙眼镜人"
```

这会在博客的页尾显示你的文章版权，留空就可以不显示。
