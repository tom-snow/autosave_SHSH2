
# autosave_SHSH2
使用 Actions 自动保存 shsh2. ([English Readme](#english-readme))

## 风险说明
本脚本行为可能违反 Github 的 TOC， 使用本脚本甚至可能会让你被封禁，请慎重使用。<br>
This script may violate Github TOC, Do not use!

## 使用说明
1. 点击右上角的 `Use this template` 以本仓库作为模版创建仓库(建议设为私有仓库).
2. 开启仓库的 actions 功能
3. 修改 [save_shsh2.yml](./.github/workflows/save_shsh2.yml) 文件中的各种变量
4. 享受自动运行的快乐。


**本程序免费[开源](https://github.com/tom-snow/autosave_SHSH2)，如果你从其他人那付费获得了 Github Action 自动保存 shsh2 的程序，那么恭喜你被骗了！**

PS: 当前不会检查历史提交的 Release，也就是说会同一个设备&版本号&G值会有多个 shsh2 文件(文件名不同)，文件内容应该完全相同的，不会影响使用。当前不打算修复，可能以后也不会去修复。

PPS: 建议也修改一下运行的时间，避免所有人都在同一时间请求 SHSH2 ，造成风控等。（每周一次的频率也足够了，太高频率没有必要，苹果更新也没那么勤，而且会消耗你的 Action 配额）

TIPS: 如果你想同时保存一个设备的最新正式版&测试版 shsh2 ，可以再复制一份 `save_shsh2.yml`，开启 beta 选项。多设备同理。 

## 参数设置
注意：对于 A12/S4 及以上设备，你必须设置 `APNONCE` + `GEN` 变量，否则生成的 shsh2 将不可用。你可以在电脑通过数据线连接到你的苹果设备，然后打开 [blobsaver](https://github.com/airsquared/blobsaver/releases)，点击 `Specify APNonce` 下的 `Read from device` 来固定与获取 `APNONCE` + `GEN` 变量。

其他参考: [tsschecker 帮助](https://github.com/1Conan/tsschecker#help)

<br><br><br><br><br><br>

# English Readme
Using actions save shsh2 automatically.

## Usage
1. Click `Use this template` to create a Repo for you (recommend private repo)
2. Enable actions
3. Modify [save_shsh2.yml](./.github/workflows/save_shsh2.yml) (The env block above)
4. Enjoy!

PS: Recommend to Modify action Schedule time, do not use default time.

## ENVS
Note: For Apple A12/S4 and newer device, you should set `APNONCE` + `GEN` variable. You can get it from [blobsaver](https://github.com/airsquared/blobsaver/releases).

Other env: [tsschecker help](https://github.com/1Conan/tsschecker#help)
