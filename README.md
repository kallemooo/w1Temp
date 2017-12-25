# w1temp_report
Simple python script that fetches temperatures from DS18B20+ 1wire sensors and pushes the data to temperatur.nu

## usage:
```
usage: w1temp_report [-h] [-s SAVE_CONFIG] [-c CONFIG] [-d]

Fetch temperatures from W1 temperature sensors and send the data to
temperatur.nu

optional arguments:
  -h, --help            show this help message and exit
  -s SAVE_CONFIG, --save_config SAVE_CONFIG
                        Store example configuration to <save_config>
  -c CONFIG, --config CONFIG
                        Configuration file <CONFIG>
  -d, --debug           set debug mode
```
## Config file example:
```ini
[DEFAULT]
baseurl = http://www.temperatur.nu/rapportera.php
connecttimeout = 30
timeout = 300

[Sensor1]
sensor = 28-0000073743b6
hash = 

[Sensor2]
sensor = 28-00000737c95d
hash = 
```
