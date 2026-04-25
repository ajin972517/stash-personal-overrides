# stash个人覆写

这是我的 Stash 个人覆写配置库，用来集中管理订阅覆写、策略组规则、分流规则、图标链接和常用片段。

## 推荐仓库英文名

GitHub 仓库名建议使用：

```text
stash-personal-overrides
```

中文项目名可以写在 README 里：`stash个人覆写`。

## 目录结构

```text
stash-personal-overrides/
├─ overrides/              # 可直接导入 Stash 的覆写文件
│  ├─ base.stoverride       # 基础通用覆写
│  ├─ google.stoverride     # Google 服务分流
│  ├─ tencent-direct.stoverride # 腾讯 / QQ / TIM 直连
│  └─ steam.stoverride      # Steam 分流
├─ snippets/               # 常用规则片段
│  ├─ domain-direct.yaml
│  ├─ domain-proxy.yaml
│  └─ reject-ads.yaml
├─ docs/                   # 使用说明
│  ├─ usage.md
│  └─ changelog.md
├─ icons/                  # 图标 URL 记录
│  └─ icon-links.md
└─ README.md
```

## 使用方式

1. 在 GitHub 新建仓库，仓库名填 `stash-personal-overrides`。
2. 把本文件包里的内容上传到仓库。
3. 打开对应 `.stoverride` 文件，复制 raw 链接。
4. 在 Stash 里添加覆写地址。
5. 后续所有规则都在这个仓库里维护，Stash 只需要更新远程覆写。

## 维护原则

- `base.stoverride` 只放全局基础设置。
- 单独功能单独文件，比如 Google、Steam、腾讯直连。
- 大改前先备份当前可用版本。
- 每次修改后，在 `docs/changelog.md` 记录日期、改动内容和测试结果。
