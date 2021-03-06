```diff
! animepahe-dlr is broken.
# :(
```
<!-- Badges -->
[![PyPI version](https://badge.fury.io/py/animepahe-dlr.svg)](https://pypi.org/project/animepahe-dlr/)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/ed-archer/animepahe-dlr/)
[![License](https://img.shields.io/github/license/ed-archer/animepahe-dlr?color=brightgreen)](https://github.com/ed-archer/animepahe-dlr/blob/main/license.md)
[![OpenIssues](https://img.shields.io/github/issues/ed-archer/animepahe-dlr?color=important)](https://github.com/ed-archer/animepahe-dlr/issues)
<!--LineBreak-->
[![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/ed-archer/animepahe-dlr/)
[![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/ed-archer/animepahe-dlr/)
<!-- Badges -->
# animepahe-dlr
A python script to automate downloads from animepahe.

## Requirements
- Python3
- FireFox Web browser

## Script dependencies
- Selenium
- BeautifulSoup4
- requests
- tqdm

## Getting Started
1. Make sure you have Python and Firefox installed in your system
2. Install PyPI package using `pip install animepahe-dlr`
3. Wait for pip to install animepahe-dlr and all required dependencies. Enjoy the script :blush:
## Usage
- Syntax: `animepahe-dlr -<optional arguments>`
- To run the script, execute `animepahe-dlr`
- To use idm to capture downloads, execute script using '-idm' argument : `animepahe-dlr -idm`

![animepahe-dlr](https://user-images.githubusercontent.com/56473062/120795797-922a3b80-c557-11eb-8328-26cfb39f4187.png)

## Features
- Search for an anime.
- Select anime from search result.
- Select episodes to download.
- Downloads are made using inbuilt-dlr (default).
- Inbuilt-dlr finds and resumes incomplete downloads by default.
- **Episode Selection Options:**
  - `0` : downloads all the episodes of the selected anime.
  - x : downloads episode x.
    - eg:- `1` : downloads episode1, `5` downloads episode5 and so on.
  - x-y : downloads episodes from x to y. 
    - eg:- `3-9` : downloads episodes 3 to 9 (3 and 9 inclusive)
  - In case of multiple options, each options must be seperated by a `,`
  - Example: `1, 3, 6-11` : downloads episodes 1,3,6,7,8,9,10,11
  
- **Downloading and Quality :**
  - Files are downloaded to your Videos directory.
  - Downloads are taken care of by the inbuilt downloader on default.
  - Currently the download quality priority is as follows : [720p, 1080p, 576p, 480p, 360p]
    - ie, downloader first checks for 720p video, if 720p is not available checks for 1080p and so on.

## Notes
- Firefox needs to be installed for this script to work (since the script uses selenium for some of its functions).
- This script is a work under progress and therefore may lack some features, please bear with it, and consider contributing if you have any fixes or improvements :relaxed:. 
- **In Windows** the webdriver if found to misbehave if the script is forced to exit using `ctrl^c`. A good solution to this couldn't be found and a temporary fix have been implemented. And as such, please be noted that if you use ctrl^c to exit, your active firefox sessions or tabs have a good chance of crashing. (Note: ctrl^c doesn't have any issues in Linux)
