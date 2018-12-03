# HQIconButton
可以自定义Button图片和标题的位置


![image](https://github.com/yanhaiqiang/HQIconButton/blob/master/image.png)

#import "UIButton+HQCustomIcon.h"

直接调用代码即可看到想要的效果
[button setIconInLeftWithSpacing:5];

不要设置按钮的宽度，如果宽度小了，文字就会变成省略号，就没效果了。
```objc
//  代码实例
_calenderButton = [UIButton buttonWithType:UIButtonTypeCustom];
[_myAssetsView addSubview:_calenderButton];
[_calenderButton autoPinEdgeToSuperviewEdge:ALEdgeTop];
[_calenderButton autoPinEdgeToSuperviewEdge:ALEdgeLeft];
[_calenderButton autoSetDimension:ALDimensionHeight toSize:44];
        
[_calenderButton setImage:kXNBImage(@"calender") forState:UIControlStateNormal];
[_calenderButton setTitle:@"日历" forState:UIControlStateNormal];
[_calenderButton setTitleColor:[UIColor blackColor] forState:UIControlStateNormal];
_calenderButton.titleLabel.font = [UIFont xnb_PingFangSCRegularOfSize:kXNFAutoValue(12)];

[_calenderButton setIconInTop];
```
