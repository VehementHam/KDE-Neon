# nala 
### Add repository 

```shell
echo "deb http://deb.volian.org/volian/ scar main" | sudo tee /etc/apt/sources.list.d/volian-archive-scar-unstable.list; wget -qO - https://deb.volian.org/volian/scar.key | sudo tee /etc/apt/trusted.gpg.d/volian-archive-scar-unstable.gpg
``` 

### Install `nala` 

```shell
apt update && sudo apt install nala
``` 

### Convert `apt` to `nala` 

Add to `~/.bashrc` and `/root/.bashrc`

```bash
alias sudo="sudo "
alias apt=nala
alias apt-get=nala
alias apt-cache=nala
```
To run an `apt` command without the alias, use the `command` argument before the command.

# firefox 

### Harden firefox

```shell
git clone https://github.com/hnhx/user.js
cd user.js
./install.sh
```
Click "Add"

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20Add%20Cropped.png)

Check "Allow this extension to run it Private Windows" then click "Okay".

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20Allow%20Extensiont%20to%20Run%20in%20Private%20Windows%20and%20Click%20Okay%20Cropped.png)

### Set default browser and search engine

Visit https://searx.work/

Enter the URL bar, type, and click the SearXNG logo with green `+` button in the top right corner.  

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Add%20SeaXNG.png)

Click the sandwitch and navigate to "Settings"

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20the%20Sandwitch%20Button%20and%20Navigate%20to%20Settings%20Cropped.png)

Click "Make Default"
![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20Make%20Default.png)

Click "Search"

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20Search.png)sponsor block

Select "searx.work"

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Click%20SearXNG.png)

### Add Sponsor Block, I don't care about cookies, and return Youtube Dislike.

Visit the Sponsor block page at https://addons.mozilla.org/en-US/firefox/addon/sponsorblock/

Click "Add"

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Sponsor%20Block.png)

There should be a pop up. When you see it, click "Add". For the next popup, check "Allow this extension to run in Private Windows" and click "Okay"

Repeat the process for the following links

I don't care about cookies: https://addons.mozilla.org/en-US/firefox/addon/i-dont-care-about-cookies/

Return Youtube Dislike: https://addons.mozilla.org/en-US/firefox/addon/return-youtube-dislikes/

### Pin Ublock Origins to toolbar

Click on the puzzle piece icon. Navigate to the Ublock Origin extention. Click on the settings icon, and check "Pin to Toolbar".

![image](https://github.com/VehementHam/KDE-Neon/blob/main/Pin%20Ublock%20Origin%20to%20Toolbar%20Cropped.png)

# Install Packages

### Install native packages

```
sudo apt install neofetch gimp freeciv make cmake gcc htop
```

## Install flatpaks

```
sudo flatpak install com.atlauncher.ATLauncher org.kde.haruna xyz.armcord.Armcord -yy
```

# Install Nvidia drivers


### Add repository

```
sudo add-apt-repository ppa:graphics-drivers/ppa -y
```

### Install drivers

```
sudo apt install xserver-xorg-video-nvidia-535 -y
```
