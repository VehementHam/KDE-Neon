# nala 
Add Repository 

```shell
echo "deb http://deb.volian.org/volian/ scar main" | sudo tee /etc/apt/sources.list.d/volian-archive-scar-unstable.list; wget -qO - https://deb.volian.org/volian/scar.key | sudo tee /etc/apt/trusted.gpg.d/volian-archive-scar-unstable.gpg
``` 

Install Nala 

```shell
apt update && sudo apt install nala
``` 

Convert `apt` to `nala` 

Add to `~/.bashrc` and `/root/.bashrc`

```bash
alias sudo="sudo "
alias apt=nala
alias apt-get=nala
alias apt-cache=nala
```
To run an `apt` command without the alias, use the `command` argument before the command.

# firefox 

Harden firefox

```shell
git clone https://github.com/hnhx/user.js
cd user.js
./install.sh
```
Click "Add"

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20Add%20Cropped.png)

Click "Allow this extension to run it Private Windows" then click "Okay".

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20Allow%20Extensiont%20to%20Run%20in%20Private%20Windows%20and%20Click%20Okay%20Cropped.png)

Visit https://searx.work/

Enter the URL bar, type, and click the green `+` button next to the SearXNG logo.  

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Add%20SeaXNG.png)

Add Sponsor Block, I don't care about cookies, Tampermonky, and return Youtube Dislike.
