# TLSDiag.ps1
This is a TLS Diagnostic tool for Windows Client/Server.

## Hot to Run This Command.
Simply run this command. It will diagnose the problem for adopting TLS 1.2.

|Parameter||Description|
|---|---|---|
|-Resolve|Switch|(Admin Privileges Required) If you would like to fix the configuration automatically, please add this switch parameter.|

### Example 1

.\TLSDiag.ps1

### Example 2 

.\TLSDiag.ps1 -Resolve

## Output

*Main Result*
|Flags|Alert Value|Description|
|---|---|---|
|TLS12Supported|False| Whether Windows OS registry configuration is configured.|
|TLS12CipherSuiteSupported|False| Whether the supported CipherSuite for M365 has been enabled.|
|TLSDotNetconfigured|False| Whether .NET 3.5 and 4.0 - 4.5 has been configured for using TLS1.2. |

We have some other sub-results that explain what was not configured.

## Reference
Please also check the following Blog Article.

https://jpdsi.github.io/blog/internet-explorer-microsoft-edge/dotnet-framework-tls12/


