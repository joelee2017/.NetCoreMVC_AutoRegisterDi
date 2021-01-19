.NetCoreMVC_AutoRegisterDi

練習自動注入

```c#
//第一種版本
// 注入 Repository
services.InJectionByGenericRepository();
 
// 注入 Service
services.InJectionByService("Service");
 
//第二種版本
// 注入 Interface
services.InJectionByInterface(new List<string>() { "Service", "Repository" });
 
// 注入 Class
services.InJectionByClass(new List<string>() { "Service", "Repository" });
 
// 注入 Generic
services.InJectionByGeneric("Model", new List<string>() { "Repository" });
```

