# powershell
https://docs.microsoft.com/en-us/powershell/

```cls``` or ```clear``` are aliases for ```Clear-Host```


```dir``` is and alias for ```Get-ChildItem```
```
PS C:\Users\rpaleru> get-ChildItem|Out-Host


    Directory: C:\Users\rpaleru


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----        3/27/2019   5:56 PM                .anaconda
d-----        9/19/2019   5:55 PM                .astropy
d-----        7/21/2020   7:04 PM                .atom
d-----        3/27/2019   3:38 PM                .cisco
d-----         4/5/2019  12:47 AM                .conda
```

```Get-Location``` returns a **PathInfo** object that contains the current path and other information.
```
PS C:\Users\rpaleru> Get-Location

Path
----
C:\Users\rpaleru
```

Piping the output to the ```Get-Member``` cmdlet displays information about the object returned by ```Get-Location```.
```
PS C:\Users\rpaleru> Get-Location|Get-Member


   TypeName: System.Management.Automation.PathInfo

Name         MemberType Definition
----         ---------- ----------
Equals       Method     bool Equals(System.Object obj)
GetHashCode  Method     int GetHashCode()
GetType      Method     type GetType()
ToString     Method     string ToString()
Drive        Property   System.Management.Automation.PSDriveInfo Drive {get;}
Path         Property   string Path {get;}
Provider     Property   System.Management.Automation.ProviderInfo Provider {get;}
ProviderPath Property   string ProviderPath {get;}
```

```
PS C:\Users\rpaleru> $PSVersionTable

Name                           Value
----                           -----
PSVersion                      5.1.17134.858
PSEdition                      Desktop
PSCompatibleVersions           {1.0, 2.0, 3.0, 4.0...}
BuildVersion                   10.0.17134.858
CLRVersion                     4.0.30319.42000
WSManStackVersion              3.0
PSRemotingProtocolVersion      2.3
SerializationVersion           1.1.0.1
```

