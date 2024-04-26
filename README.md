## 初始化项目

```
hugo new site my_website
cd my_website
```

## 主题

```
git init
git submodule add https://github.com/HEIGE-PCloud/DoIt.git themes/DoIt
```

## 配置目录

```
├── config
│   ├── _default
│   │   ├── hugo.toml
│   │   ├── languages.toml
│   │   ├── menus.en.toml
│   │   ├── menus.zh.toml
│   │   └── params.toml
│   ├── production
│   │   ├── hugo.toml
│   │   └── params.toml
│   └── staging
│       ├── hugo.toml
│       └── params.toml
```

考虑上面的结构，当运行 hugo --environment staging 时，Hugo 将使用 config/_default 中的所有设置，并将 staging 的设置与之合并。

