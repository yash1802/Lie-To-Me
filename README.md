# Lie-To-Me
A machine learning based lie detector primarily built for fact checking in the context of politics.

## How it works.
Via a built-in scraper, it collects data, a "data of lies" if you will, from "politic fact" (http://www.politifact.com/truth-o-meter/statements). 
A neural network is trained using this data and given an arbitrary statement from the news, it determines whether or not the said statement is true.

## How to use.
from data import Scrape

### If the data is already on the disk, `Scrape.read() `will just process that, else the data will be scraped.'''
my_scraped_data = Scrape.read()

### Cleans as well as vectorizes the data and puts stores it in the data structure.
processed_data = Process.data_init(my_scraped_data) 
