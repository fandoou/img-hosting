# `FanDou`的图床

## 搭建步骤

1. **创建仓库**

   创建一个 `git` 仓库用于存储图片。目录结构如下：

   ```shell
   ├─common
   ├─draw.io
   ├─front-end
   │  └─vue.js
   │      ├─vue
   │      ├─vue-router
   │      └─vuex
   └─wallpaper
   ```

   - 生成目录结构：打开命令行工具，进入根目录输入 `tree` 命令即可。

2. **引用图片**

   ```
   https://cdn.jsdelivr.net/gh/fandoou/img_hosting/详细路径
   ```

---

## 管理图片

### `PicGo`

可以使用 `PicGo` 来管理 `GitHub` 图床。

1. **`GitHub`配置**

   依次点击 `User` - `Settings` - `Developer settings` - `Personal access tokens`，选择 <kbd>Generate new token</kbd>，填入以下信息，创建一个新的个人访问令牌：

   - **`Note`**：图床仓库地址（直接填写仓库名称）
   - **`Select scopes`**：选择 `repo` 中的全部选项

   拷贝生成的 `Token` 值，并保存在一个私密的地方。

2. **`PicGo`设置**

   打开 `PicGo`，点击“图床设置”，选择 ”`GitHub`图床“，填入以下信息：

   | 信息名称       | 填入内容                                        |
   | -------------- | ----------------------------------------------- |
   | 设定仓库名     | `username/respository-name`                     |
   | 设定分支名     | `master`                                        |
   | 设定`Token`    | 生成的 `Token`                                  |
   | 指定存储路径   | 任意填写                                        |
   | 设定自定义域名 | `https://cdn.jsdelivr.net/gh/用户名称/仓库名称` |

---

## 壁纸尺寸

| 分辨率          | 描述       | 比例    |
| --------------- | ---------- | ------- |
| `1280` × `720`  | `720P`     | `16:9`  |
| `1920` × `1080` | `1080P`    | `16:9`  |
| `2048` × `1080` | `WQHD`     | `≈17:9` |
| `3840` × `2160` | `UHD`      | `16:9`  |
| `4096` × `2160` | `Ultra HD` | `≈17:9` |

---

