# Debian-ReInstall
NETINSTALL:     
It can reinstall Debian(Ubuntu) from CentOS/Ubuntu/Debian         

Link to: [Debian(Ubuntu)网络安装/重装一键脚本](https://moeclub.org/2017/03/25/82/)     

--------------------------------------------------------------  
--------------------------------------------------------------  
# Description
Apply to CentOS, Ubuntu, Debian that is booted by the GRUB.      
As long as you have root permissions, you also have a pure system.        
Not suitable for OPENVZ.    
  
Default root password is 'Vicer'      
Please change it as soon as possible.     

--------------------------------------------------------------    
--------------------------------------------------------------   
    
# Usage
```
bash DebianNET.sh       -d/--debian/--ubuntu [Dist Version Name]
                        -v/--ver [32/i386|64/amd64]
                        --mirror '[Mirror Server]'
                        -a/-m
```
                        

```
-----------------------------------------    
| Dists   |  Version    |  Version Name |  
-----------------------------------------    
| Debian  |   7         | wheezy        |   
|         |   8         | jessie        |
|         |   9         | stretch       | 
-----------------------------------------    
| Ubuntu  |   12.04     | precise       |
|         |   14.04     | trusty        |
|         |   15.10     | wily          |
|         |   16.04     | xenial        | 
|         |   16.10     | yakkety       | 
|         |   17.04     | zesty         |
-----------------------------------------      
```
--------------------------------------------------------------    
--------------------------------------------------------------    

# Example
First
```
wget --no-check-certificate -qO DebianNET.sh 'https://moeclub.org/attachment/LinuxShell/DebianNET.sh' && chmod -x DebianNET.sh
```
Then
```
bash DebianNET.sh -d trusty -v i386 -a
```
```
bash DebianNET.sh -d stretch -v amd64 -a --mirror 'http://mirrors.ustc.edu.cn/debian/'
```
