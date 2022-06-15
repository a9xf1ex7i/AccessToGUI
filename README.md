# AccessToGUI - for service only
This library allows the service to run any processes with administrator rights.

### Usage example
```c#
protected override void OnStart(string[] args)
{
    AccessToGUI.Application.PROCESS_INFORMATION info;
    var result = AccessToGUI.Application.StartProcess("cmd.exe", out info);
}
```
This code will open a command prompt with administrator rights when the service is started.
