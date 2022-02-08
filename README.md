# 为什么会有这个仓库
* 用unity自带的upm下载是在Library文件夹里，由于Library文件夹一般都会用gitignore忽略掉，本地修改了源码其他人也拉取不到，索性自己建个仓库维护。
# 与原版的差别
* 主要是对[TMP_Text.cs](https://github.com/0kk470/textmeshpro1.5.0/blob/main/Scripts/Runtime/TMP_Text.cs#L1268) 进行了修改，增加了一个 <b>OnMaterialAssetRequest</b> 回调，使得 <material>标签 支持从诸如AssetBundle这类自定义接口加载材质（原代码只能从Resource目录下加载）。
