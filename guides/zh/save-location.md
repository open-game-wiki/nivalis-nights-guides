---
title: "存档位置、手动保存与备份"
description: "查找 Nivalis Nights 官方 Windows 存档目录，备份 .sav 文件，了解手动保存和 Steam 云存档，恢复前先保留当前进度。"
category: "Technical"
publishDate: "2026-10-16"
updatedDate: "2026-10-16"
lang: "zh"
---

## Windows 存档位置
505 Games 给出的日志与 `.sav` 文件目录是：

```text
%USERPROFILE%\AppData\LocalLow\ION LANDS\Nivalis Nights
```

按 **Win + R**，粘贴路径后回车。`.sav` 是存档；同目录下的 `Player.log` 和 `Player-prev.log` 是诊断日志，不是存档。

## 修改前怎样备份
1. 从暂停菜单手动保存，再正常关闭游戏。
2. 把整个存档目录复制到单独的日期文件夹。使用复制，不要移动原文件。
3. 备份放在游戏活动目录以外。测试模组或恢复旧文件前，再保留一份当前状态。
4. 恢复时保持游戏关闭，核对准备替换的文件。重启后检查日期、店铺和任务是否符合预期，再继续游玩。

Steam 云存档用于同步，不能替代自己的分日期备份。发生云同步冲突时先看时间戳并保留本地候选文件，再选择保留哪个版本；排查进度丢失时不要反复覆盖同一个文件。

## 手动保存与自动保存
开发者 FAQ 说明：游戏在每天结束时自动保存，也可从暂停菜单手动保存。退出前手动保存，可保留上次日末自动保存之后的进度；云同步需要网络连接。

## 保存失败怎么办
记下报错、涉及的槽位或文件、上次成功保存的时间。尝试恢复前留一份未修改副本。问题反复出现时联系 [505 Games 支持](https://support.505games.com/)，按要求提供日志；只有支持人员要求时再提供存档，不要公开上传整个目录。

## 来源
- [505 Games 存档与日志位置](https://support.505games.com/support/solutions/articles/150000235215-please-read-this-if-you-have-an-issue-playing-nivalis-nights)，核对于 2026-10-16。
- [开发者 FAQ：保存](https://steamcommunity.com/app/1488490/discussions/0/598530855994991183/)。
