Usage

Simply clone this repository and run:

docker-compose up -d



What To Do Next


Try Nmap
```bash
sudo nmap -Pn -p 3389 172.17.0.2
```

or 

Install an RDP client of your choice for Linux. A popular one is RDesktop:

```bash
sudo apt-get install rdesktop
```

Finally, we can access the Windows VM:
```bash
sudo rdesktop 172.17.0.2
```


Creds 

The Windows box that we have installed has two built-in accounts:

Username: vagrant Password: vagrant
Username: Administrator Password: vagrant