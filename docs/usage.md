# 使用说明

## 1. 如何添加到 Stash

进入 Stash：

```text
设置 / 配置 / 覆写 / 添加远程覆写
```

粘贴 GitHub Raw 链接，例如：

```text
https://raw.githubusercontent.com/你的用户名/stash-personal-overrides/main/overrides/base.stoverride
```

## 2. 文件拆分建议

建议不要把所有规则塞进一个文件。后续维护时可以这样拆：

- `base.stoverride`：全局基础设置
- `google.stoverride`：Google 全家桶
- `tencent-direct.stoverride`：腾讯 / QQ / TIM 直连
- `steam.stoverride`：Steam 分流
- `ai.stoverride`：AI 平台
- `payment.stoverride`：支付 / 订阅平台

## 3. 修改规则后的检查

每次改完后：

1. 确认 YAML 缩进正确。
2. 确认策略组名称和订阅内完全一致。
3. 在 Stash 里更新远程覆写。
4. 观察是否报错。
5. 测试常用网站和 App。
