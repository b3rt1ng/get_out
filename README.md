![linux_only](https://badgen.net/badge/made%20for/Linux/red) ![python_version](https://badgen.net/badge/python/3.7/yellow) ![console_only](https://badgen.net/badge/icon/terminal%20only/pink?icon=terminal&label)
# 🌌 NOVA 🌌
NOVA is under heavy developement for the moment and the arp poisoning isn't working proprely yet.  
The script will allow you to perform ARP poisoning by analysing your network and showing who is avariable.  
Right now, NOVA is only performing an accurate and fast network scan.
# ☄️ installation ☄️ 
```
git clone https://github.com/b3rt1ng/NOVA.git
cd get_out/
chmod +x install.sh
./install.sh
```  
You'll need to install [scapy](https://scapy.net/) in order to perform all the differents attacks
# 🌟 usage 🌟
```
python3 main.py [argument]
``` 
| Argument | Description |
| --- | --- |
| -i | allow you to set up a custom interface by name if the script don't find anything on monitor mode |
| -pt "value" | set a value to change the delay to wait the pings results |
| -ip "local ip" | this command allow you to set you local ip manually if the script have trouble while finding it |
| -h | show the help menu |
| --debug | The script will wait for you to continue before displaying the menu, it's easyer to see what it does |  
  
  (You can use any argument at the same time)

## ✨ Next updates ✨
  
* ability to save the host list to use it on another program (and maybe load it back)
* ability to send maliscious packet like deauth or arp spoof
* listen to the network and save the currents hosts by time to render a graphic and data analytics from it

### ⭐ what do you need to run this program ⭐

You need to have [scapy](https://scapy.net/) for python3.  

if you didn't get the wireshark OUI database by running the install file: 
[Here it is](https://gitlab.com/wireshark/wireshark/raw/master/manuf)

### 💫 Is there something you will improve 💫
Improvement done:  
- fast nework scan
- detect the gateway
- detect interface in monitor mode  

Work in progress:  
The network scan launch some thread to know wich ip is up on the network. some ping might take longer that expected and sometime you will miss some hosts. I plan on making a verbose system later to adjust it manually.  
  
For the moment it only scan your network, there is no arp spoof or deauth system. I try to make it as simple as possible and easy to use. I don't wan to use too much external library to make it accessible and easy to modify for anyone from beginner to advanced programmer.  
  
Because I want the script to be easy to modify and understandale to everyone, I do not make my programming object oriented. sorry :(
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Do not use this script for any illegal purposes.

