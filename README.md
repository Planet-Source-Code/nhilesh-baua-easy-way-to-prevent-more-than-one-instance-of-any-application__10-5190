<div align="center">

## Easy Way to prevent more than one instance of any application


</div>

### Description

This tutorial will help, preventing more then one instance of any application, which contains this code in form_load event.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nhilesh Baua](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nhilesh-baua.md)
**Level**          |Intermediate
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |C\#
**Category**       |[Debugging and Error Handling](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/debugging-and-error-handling__10-6.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nhilesh-baua-easy-way-to-prevent-more-than-one-instance-of-any-application__10-5190/archive/master.zip)





### Source Code

```
bool isInstanceExisting= false;
Mutex objMutex = new Mutex true, "Application_Mutex", out isInstanceExisting);
if (!isInstanceExisting)
{
 this.Dispose();
 return;
}
```

