# CSChannelLabelView-OC
一个轻量的文字频道View。多个频道可滚动，少量频道可适配间距。
本版本为[Objective-C版](https://github.com/JoslynWu/CSChannelLabelView-OC.git)。

## Swift版入口：[CSChannelLabelView](https://github.com/JoslynWu/CSChannelLabelView)

## 效果图
![](/Effect/CSChannelLabelView.gif)

## 怎么接入

直接将Sources文件夹拖入工程中。


## 怎么用

- 建议属性设置完后，再调用刷新方法。

```Objective-C
- (void)refreshTitles:(NSArray<NSString *> *)titles;
```

- 下面方法一般在代码调用时调用，例如滚动UICollectionView时需要title同时滚动

```Objective-C
- (void)selectChannelWithIndex:(NSInteger)index animated:(BOOL)flag;
```

- 选择指示器支持多种动画类型

```Objective-C
typedef NS_ENUM(NSInteger, CSIndicatorAnimationType){
    CSIndicatorAnimationTypeNone,       // 无动画
    CSIndicatorAnimationTypeSlide,      // 滑行动画
    CSIndicatorAnimationTypeCrawl,      // 爬行动画
    CSIndicatorAnimationTypeRubber,     // 橡胶动画
};
```
