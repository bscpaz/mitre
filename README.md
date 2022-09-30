<h1 align="center">MITRE ATT&amp;CK</h1>
<p align="center">This page is about cybersecurity</p>

See more:

https://attack.mitre.org/

https://portswigger.net/web-security

https://www.youtube.com/watch?v=FSjOrIHun-A

## Advanced persistent threat (APT)
_"An advanced persistent threat (APT) is a sophisticated, sustained cyberattack in which an intruder establishes an undetected presence in a network in order to steal sensitive data over a prolonged period of time"_.

### Windows
#### Disable or Remove Feature or Program
https://attack.mitre.org/mitigations/M1042/

##### PowerShell/WinRM

* If you want to stop and disable the WinRM for security reasons, you can do so in the Services snap-in (type "services" in the start menu), or you can use PowerShell:

  ```shell 
  Stop-Service WinRM -PassThruSet-Service WinRM -StartupType Disabled -PassThru
  ```
  
  * For test:
  
  ```shell
  Test-WSMan localhost
  ``` 
