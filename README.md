# Minecraft log parser
The purpose of this project is that minecraft server administrators get insight into how much, when and by whom their server gets used. It also provide other information.

## Planned data to parse
The things listed below are features that will be implemented and are planned from the start.
- Chat messages including player name and date/time
- Player deaths
- Player kills
- Play time per player

## Possible data to parse in the future 
The things listed below are features that may get added in the future but are of low priority. These features also aren't certain if they will get added.
- Player achievements
- Server crashes
- Server timeouts
- Players banned
- Commands ran

## Usage
There are multiple scripts that get used for the process of analyzing the log files. 
The first step is to concatenate all of the log files together and add distinguishable dates into the file. 
The second step is to parse this one big log file and extract the useful information and save this in multiple csv files. 
The third and final step is to analyze the data that was extracted using the R programming language.

### concat.py:
concat.py is a python script for concatting multiple log files. When you want to use the parser for multiple days of server logs you should first use this script.


### extractData.py:
This python script extracts data fromm the log files. See below for which data it will extract.
