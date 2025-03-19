# Seje2

![screenshot](screenshot.png)

[Demo](https://eatradish.github.io/Seje2)
[简体中文](https://github.com/eatradish/Seje2/blob/main/README_zh_cn.md)

## Installation
First download this theme to your `themes` directory:

```bash
cd themes
git clone https://github.com/eatradish/Seje2
```
and then enable it in your `config.toml`:

```toml
theme = "Seje2"
```

This theme requires your index section (`content/_index.md`) to be paginated to work:

```toml
paginate_by = 5
```

The posts should therefore be in directly under the `content` folder.

and requires your index section (`about/_index.md`) to be paginated to work:

```toml
title = "..."

[extra]
year = 2019
month = 11
day = 3
```

## Options

### Top-menu
Set a field in `extra` with a key of `seje2_menu_links`:

```toml
seje2_menu_links = [
    {url = "$BASE_URL", name = "Home"},
    {url = "$BASE_URL/categories", name = "Categories"},
    {url = "$BASE_URL/tags", name = "Tags"},
    {url = "https://google.com", name = "Google"},
]
```

If you put `$BASE_URL` in a url, it will automatically be replaced by the actual
site URL.

### MathJax Latex Support
Set a field in `extra` with a bool key of `seje_mathjax`:

```toml
seje_mathjax = true
```

### License

Set a field in `extra` with a key of `license`:

```toml
license = "@ 宇宙眼镜人"
```
