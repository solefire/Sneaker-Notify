**Donation:**
Feel free to buy me a cup of coffee, so I can stay motivated and keep updating this project.

[![PayPal](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=3WA5WTGP9HPYG)

#
Sneaker/Restock/Monitor Notify via Twitter coded in Python using Scrapy.

![Example](http://i.imgur.com/cqI2s0x.png)
#
Status: **Under Development. If Interested feel free to [![Twitter Follow](https://img.shields.io/twitter/follow/espadrine.svg?style=social&label=Follow)](https://twitter.com/w_notify) on Twitter. To view the database online check [here](https://shoesaddictor.com/Crawler_DB.php).**

Description: Crawl a list of sneaker websites. Once the new product is found or is restocked. It will check the item's name for certain keywords. If found, it will alert the user via Twitter using tweets, with date, time, item name, and link.
#
**Supported Sites List:**
 - 43einhalb
 - 5 Pointz
 - AFewStore
 - ALLike
 - Addict
 - Adidas
 - Aphrodite
 - AsphaltGold
 - BSTN
 - Back Door
 - Bait
 - Barneys - Ban if crawl too much.
 - Basket Store
 - Blends
 - Bodega
 - Caliroots
 - Capsule
 - ChampsSports
 - City Gear
 - Concepts
 - Consortium
 - DeadStock
 - DefShop
 - Dope Factory
 - Drome
 - DSMNY
 - EastBay
 - End - Captcha if crawl too much.
 - Extra Butter NY
 - Feature
 - FinishLine - Banned on Vultr.
 - FootAction
 - FootAsylum
 - FootDistrict
 - FootLocker
 - FootPatrol
 - FootShop
 - Hanon
 - Haven
 - HypeBeast
 - HypeDC
 - Inflammable
 - JDSports
 - JimmyJazz - ASN blocked on Vultr via CloudFlare.
 - Kith
 - Kong
 - Lapstone and Hammer
 - Loaded
 - Luisa Via Roma
 - MrPorter
 - NeedSupply
 - Next Door
 - NiceKicks
 - Nike
 - Nordstrom
 - Notre
 - Nrml
 - Office
 - Offspring
 - Oneness
 - OverKill
 - Packer
 - Proper
 - Puff Reds
 - Renarts
 - Rise45
 - Ruvilla
 - SSense
 - SVD
 - SaintAlfred
 - SaveOurSole
 - Shelf Life
 - ShoesPalace - Need to disobey robots.txt, if you want to crawl.
 - Size
 - Slam Jam Socialism
 - SneakerBaas
 - SneakerNStuff - ASN blocked on Vultr via CloudFlare.
 - SneakerPolitics
 - SocialStatus
 - SoleBox
 - SoleKitchen
 - SoleStop
 - Solefly
 - StickABush
 - StormFashion
 - Summer
 - Tint Footware
 - Titolo
 - Tres Bien
 - TrophyRoom
 - Undefeated
 - Uptown
 - Urban Industry
 - Urban Jungle
 - Urban Outfitters
 - WellGosh
 - West NYC
 - XileClothing
 - YCMC
 - YME Universe
 - Zappos
#
**Requirements:**
- pip install scrapy
- pip install scrapy-random-useragent
- pip install TwitterAPI
- pip install crayons
- pip install datetime
- pip install beautifulsoup4
- pip install pypiwin32
- pip install MySQL-python
- pip install mysql-connector
#
**Setup:**
1. Make sure you have Python installed. (Working on Python 2.7 - not working on Python 3) To install Python go to https://www.python.org/

2. Install the pip requirements above.
- For Mac: to install MySQL-python. Open terminal and type the below:
```
 - /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
 - brew install mysql-connector-c
 - pip install MySQL-python
```

If you have problem installing mysqldb or getting "no module named mysqldb" for Windows go to: http://www.lfd.uci.edu/~gohlke/pythonlibs/#mysql-python

```
Download:
MySQL_python‑1.2.5‑cp27‑none‑win32.whl for 32 Bit
MySQL_python‑1.2.5‑cp27‑none‑win_amd64.whl for 64 Bit

pip install wheel
pip install MySQL_python‑1.2.5‑cp27‑none‑win32.whl for 32 Bit
pip install MySQL_python‑1.2.5‑cp27‑none‑win_amd64.whl for 64 Bit
```

3. Install the MySQL database -> .sql file provided in the folder.

4. Go into mysql_pipeline.py edit MySQL connection info and edit Twitter's CONSUMER_KEY, CONSUMER_SECRET, ACCESS_TOKEN_KEY, and ACCESS_TOKEN_SECRET to your Twitter account's info.

5. To run:
 - For Windows: Click on main.py
 - For Mac: Open terminal on the folder type python main.py
 
Optional: Added a crawler_db.php to see the data online.
 - To install, put crawler_db.php on your web server with the crawler's database running and edit the connection info.