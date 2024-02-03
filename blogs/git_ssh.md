## Link git to github
- ssh-keygen -t rsa -b 4096 -C "1926487130@qq.com"

- GitHub配置公钥

- cd ~/.ssh/

- vim config

- config 包含如下内容：
Host github.com
User L7991-lian
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_rsa
Port 443

- ssh-add id_rsa

- ssh -T git@github.com
