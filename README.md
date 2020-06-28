<h1 align="center">
  <br>
  <a href="https://github.com/cantixcrew/s1cans"><img src="https://github.com/cantixcrew/s1cans/blob/master/img/1593113761752.png" alt="s1cans"></a>
  <br>
  VulnX
  <br>
</h1>
[![Python 3.x](https://img.shields.io/badge/python-3.6%7C3.7-yellow.svg)](https://www.python.org/) 
![Size](https://img.shields.io/github/size/cantixcrew/s1cans/README.md)
![Tweet](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fnenghaxor)
![Follow](https://img.shields.io/twitter/follow/nenghaxor?label=Follow&style=social)

### FEATURES SCAN:
- [x] Subdomain
- [x] Folder
- [x] Github account

### INSTALATION:
git clone https://github.com/cantixcrew/s1cans.git

cd s1cans

pip3 install -r requirements.txt

### USAGE:

Short Form    | Long Form     | Description
------------- | ------------- |-------------
-u            | --url         | URL in which you want to find (sub)domains.
-l            | --listfile    | File which contain list of URL's needs to be scanned.
-o            | --output      | Output file name in which you need to save the results.
-c            | --cookie      | Cookies which needs to be sent with request.
-h            | --help        | show the help message and exit.
-d            | --domain      | Give TLD (eg. for www.example.com you have to give example.com) to find subdomain for given TLD.
-g            | --gitscan     | Needed if you want to get things via Github too.
-gt           | --gittoken    | Github API token is needed, if want to scan (also needed -g also).
-f            | --folder      | Root folder which contains files/folder.

### Examples
* To list help about the tool:
```
python3 s1cans.py -h
```
* To find subdomains, s3 buckets, and cloudfront URL's for given single URL:
```
python3 s1cans.py -u http://www.example.com
```
* To find subdomains from given list of URL (file given):
```
python3 s1cans.py -l list.txt
```

* To save the results in (output.txt) file:
```
python3 s1cans.py -u https://www.example.com -o output.txt
```
* To give cookies:
```
python3 s1cans.py -u https://www.example.com -c "test=1; test=2"
```
* To scan via github:
```
python3 s1cans.py -u https://www.example.com -o output.txt -gt <github_token> -g 
```
* Folder Scanning:
```
python3 s1cans.py -f /path/to/root/rexa@dev/labs/sicans/  -d example.com  -gt <github_token> -g
```
