# CSChannelTitleView-OC
一个轻量的文字频道View。多个频道可滚动，少量频道可适配间距。
本版本为[Objective-C版](https://github.com/JoslynWu/CSLabelTitleView-OC.git)。

## Swift版入口：[CSChannelView](https://github.com/JoslynWu/CSLabelTitleView)

## 效果图
![](/Effect/CSChannelTitleView.png)

## 怎么接入

直接将Sources文件夹拖入工程中。

## 使用说明

- 建议属性设置完后，再调用刷新方法。

```
- (void)refreshTitles:(NSArray<NSString *> *)titles;
```

- 下面方法一般在代码调用时调用，例如滚动UICollectionView时需要title同时滚动

```
- (void)selectLabelWithIndex:(NSInteger)index animated:(BOOL)flag;
```

