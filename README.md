# PaimonsNotebookResources

原神工具箱 [PaimonsNotebook](https://github.com/shadyrispy/PaimonsNotebook) Android 客户端的静态资源 CDN 镜像仓库。

通过 [jsDelivr](https://www.jsdelivr.com/) 全球 CDN 提供稳定快速的资源访问。

## 资源结构

仓库按 14 个分类目录组织：

| 分类 | 文件数 | 用途 |
|------|--------|------|
| AchievementIcon/ | 77 | 成就图标 |
| AvatarCard/ | 142 | 角色卡片 |
| AvatarIcon/ | 320 | 角色头像 |
| Bg/ | 535 | 背景图 |
| ChapterIcon/ | 164 | 章节图标 |
| EmotionIcon/ | 761 | 表情图标 |
| EquipIcon/ | 609 | 武器图标 |
| ItemIcon/ | 2542 | 材料/物品图标 |
| Mark/ | 314 | 地图标记 |
| MonsterIcon/ | 350 | 怪物图标 |
| NameCardPic/ | 547 | 命名卡片 |
| RelicIcon/ | 562 | 圣遗物图标 |
| Skill/ | 1614 | 技能图标 |
| Talent/ | 1178 | 天赋图标 |

**总计：9,715 个 PNG 文件 (~732MB)**

## 访问方式

通过 jsDelivr CDN 访问任意资源：

```
https://cdn.jsdelivr.net/gh/shadyrispy/PaimonsNotebookResources@main/{category}/{fileName}.png
```

### 示例

- 角色头像: https://cdn.jsdelivr.net/gh/shadyrispy/PaimonsNotebookResources@main/AvatarIcon/UI_AvatarIcon_Zhongli.png
- 武器图标: https://cdn.jsdelivr.net/gh/shadyrispy/PaimonsNotebookResources@main/EquipIcon/UI_EquipIcon_Sword_Blunt.png
- 圣遗物图标: https://cdn.jsdelivr.net/gh/shadyrispy/PaimonsNotebookResources@main/RelicIcon/UI_RelicIcon_15001_1.png
- 怪物图标: https://cdn.jsdelivr.net/gh/shadyrispy/PaimonsNotebookResources@main/MonsterIcon/UI_MonsterIcon_Dvalin.png

## 数据来源

镜像自 [Snap.Hutao.Remastered](https://github.com/SnapHutaoRemasteringProject/Snap.Hutao.Remastered) 项目的 API:
- 原 API: `https://api.snaphutaorp.org/static/raw/{category}/{fileName}.png`
- 本仓库: `https://cdn.jsdelivr.net/gh/shadyrispy/PaimonsNotebookResources@main/{category}/{fileName}.png`

## 应用集成

在 PaimonsNotebook 项目中通过 `HutaoEndpoints.kt` 配置使用:

```kotlin
private const val ApiSnapHutao = "https://cdn.jsdelivr.net/gh/shadyrispy/PaimonsNotebookResources@main"
const val ApiSnapGenshinStaticRaw = ApiSnapHutao
```
