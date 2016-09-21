# webviewTest
抓取webview 元素 请求头相应头

集成方法
```

1、#import "FilteredWebCache.h"

2、
     NSArray *paths=NSSearchPathForDirectoriesInDomains(NSDocumentDirectory, NSUserDomainMask, YES);
    NSString *documentPath=[paths objectAtIndex:0];
    NSUInteger discCapacity = 10*1024*1024;
    NSUInteger memoryCapacity = 512*1024;
    _cache =
    [[FilteredWebCache alloc] initWithMemoryCapacity: memoryCapacity
                                        diskCapacity: discCapacity diskPath:documentPath];
    [NSURLCache setSharedURLCache:_cache];
   
  
```

