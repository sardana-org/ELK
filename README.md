# ELK-sardana

Contains configuration an filter files used for ELK deployment on the beamlines. ( Currently on test state )

# Installation guide

Install the ELK packages you require according to your OS
Example:
[Filebeat installation example](https://www.elastic.co/guide/en/beats/filebeat/6.8/filebeat-installation.html)

Clone this repository in your folder of preference
```
git clone
```
After installing you can find the config for the packages in:
```
/etc/"package name"
ex: /etc/filebeat
```
Copy as superuser the files from this repo to the folders containing the packages config files. The system needs sudo permision on this config files.
Example:
```
sudo cp filebeat/filebeat.yml /etc/filebeat/filebeat.yml
```

Restart the services and they should acquire the configuration from the repo
At last, change the .yml files to config your network IPs
