# ZKSlideViewController
微博发现模块左右滑动 ViewController 效果

![intro.gif](https://github.com/dev-zhoukang/ZKSlideViewController/blob/master/Source/intro.gif)

### 使用方法
1. 创建一个容器控制器，继承自`ZKSlideViewController`
2. 初始化子控制器

```
- (void)viewDidLoad {
    [super viewDidLoad];
    [self setupChildViewControllers];
}

- (void)setupChildViewControllers {
    ZKHotViewController *hotVC = [ZKHotViewController new];
    hotVC.title = @"热门";
    [self addChildViewController:hotVC];
    
    ZKListViewController *listVC = [ZKListViewController new];
    listVC.title = @"榜单";
    [self addChildViewController:listVC];
    
    ZKVideoViewController *videoVC = [ZKVideoViewController new];
    videoVC.title = @"视频";
    [self addChildViewController:videoVC];
}
```
