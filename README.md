# autosave_SHSH2
使用 Actions 自动保存 shsh2. ([English Readme](#english-readme))

## 使用说明
1. 点击右上角的 `Use this template` 以本仓库作为模版创建仓库(建议设为私有仓库).
2. 开启仓库的 actions 功能
3. 修改 [save_shsh2.yml](./.github/workflows/save_shsh2.yml) 文件中的各种变量
4. 享受自动运行的快乐。


## 参数设置
注意：对于 A12/S4 及以上设备，你必须设置 `APNONCE` 变量，否则生成的 shsh2 将不可用。你可以在电脑通过数据线连接到你的苹果设备，然后打开 [blobsaver](https://github.com/airsquared/blobsaver/releases)，点击 `Specify APNonce` 下的 `Read from device` 来获取 `APNONCE` 变量。

其他参考: [tsschecker 帮助](https://github.com/1Conan/tsschecker#help)

<br><br><br>

# English Readme
Using actions save shsh2 automatically.

## Usage
1. Click `Use this template` to create a Repo for you (recommend private repo)
2. Enable actions
3. Modify [save_shsh2.yml](./.github/workflows/save_shsh2.yml) (The env block above)
4. Enjoy!

## ENVS
Note: For Apple A12/S4 and newer device, you should set `APNONCE` variable. You can get it from [blobsaver](https://github.com/airsquared/blobsaver/releases).

Other env: [tsschecker help](https://github.com/1Conan/tsschecker#help)
