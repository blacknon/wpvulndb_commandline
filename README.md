# wpvulndb_cmd
A commandline vulnerability reporter using WP-CLI and WPVulnDB

# Usage

Specially useful for server admin's managing the wordpress backend and what a quick list of vulnerable plugin's. Running wpscan is a tiresome process and does non needed bruteforce. Being a server admin the list of plugin's / themes could be directly extracted.

# CommandLine Options

``usage: wpscancli.py [-h] --path PATH [--vulnonly]

This program is used to run a quick wordpress scan via wpscan api. This
command depends on wp-cli

optional arguments:
  -h, --help   show this help message and exit
  --path PATH  Provide URL
  --vulnonly   Only List vulnerable Plugins

Credit (C) Anant Shrivastava http://anantshri.info``


## Basic working
Wordpress management part is handed over to WP-CLI as it is doing its job too well.  The list of plugin's and version's obtained from wp-cli are then used to extract results from wpvulndb.


## To-do
1. add support for wordpress version specific issues reporting
2. add support for theme vulnerability scanning
3. export report in csv/xml/json format