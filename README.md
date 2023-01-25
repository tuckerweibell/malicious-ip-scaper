# Malicious IP Scraper
This is a public IP scaper that may be used to compile large lists of known malicious IP addresses into CSV files. The scraper pulls the latest OSINT data from Firehol and AbuseIPDB and parses IP addresses and IP CIDR ranges into CSV lists that may be imported into SIEMs, EDR systems, or WAFs to detect or prevent malicious activity in your environment.

## Get Started

1. Clone repository.
2. Install [ruby](https://www.ruby-lang.org/en/documentation/installation/) on your host.
3. Add executable permissions to the scrape_all.sh file.
4. Execute the scrape_all.sh (on windows you will need “Windows Subsystem for Linux” to run .sh files)


### Example

Assuming you have ruby installed and you are running on Linux or MacOs...

```
git clone git@github.com:tuckerweibell/malicious-ip-scaper.git
```

```
cd malicious-ip-scraper
```

```
chmod 777 scrape_all.sh
```

```
./scrape_all.sh
```

```
➜  malicious-ip-scaper git:(main) ✗ ./scrape_all.sh 
Pulled data from page=1 successfully.
Pulled data from page=2 successfully.
Pulled data from page=3 successfully.
...
```
