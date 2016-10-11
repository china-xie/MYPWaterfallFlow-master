# MYPWaterfallFlow---


1.
//跟随着父控件的尺寸而自动伸缩
waterflowView.autoresizingMask = UIViewAutoresizingFlexibleWidth | UIViewAutoresizingFlexibleHeight;



2.
if (UIInterfaceOrientationIsPortrait(self.interfaceOrientation)) {//竖屏
    return 3;
}else{
    return 5;
}


3.横屏、竖屏适配
/**
 *  屏幕旋转完毕时调用
 */
- (void)didRotateFromInterfaceOrientation:(UIInterfaceOrientation)fromInterfaceOrientation
{
    NSLog(@"屏幕旋转完毕");
}

//跟随着父控件的尺寸（宽度、高度）而自动伸缩
waterflowView.autoresizingMask = UIViewAutoresizingFlexibleWidth | UIViewAutoresizingFlexibleHeight;


if (UIInterfaceOrientationIsPortrait(self.interfaceOrientation)) {//如果是竖屏
    return 3;
}else{
    return 5;
}
