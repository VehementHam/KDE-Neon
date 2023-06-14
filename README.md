# nala 
Add Repository 

```shell
echo "deb http://deb.volian.org/volian/ scar main" | sudo tee /etc/apt/sources.list.d/volian-archive-scar-unstable.list; wget -qO - https://deb.volian.org/volian/scar.key | sudo tee /etc/apt/trusted.gpg.d/volian-archive-scar-unstable.gpg
``` 

Install Nala 

```shell
apt update && sudo apt install nala
``` 

Convert APT to Nala 
add to `~/.bashrc` and `/root/.bashrc`

```bash
alias sudo="sudo "
alias apt=nala
alias apt-get=nala
alias apt-cache=nala
```
# firefox 

Visit [(https://searx.work/)]

