# Dynamic_Scraper_with_AgentQL-ScrapeGraph
## What is this?
This is a web scraping tool that is AI powered, and can be used to extract information dynamically from web pages. It automatically 
detects pagination, and should be able to scrape most websites on multiple pages by it self. 

## Set up the .env file:
If you dont have a .env file, create one by copying the .env.example file and filling in the details

## Installation
1. on windows, make a python virtual environment, do it in *command prompt*:
```python
python -m venv env
```
2. Activate the virtual environment:
```python
.\env\Scripts\activate
```

3. Install the required dependencies using `pip install -r requirements.txt`


## Usage
1. Create a configuration file as described in AnExample_CONFIG_FILE.yml
2. Run the tool using `python main.py`, make sure to have the config file correctly set up
3. The tool will scrape the specified URLs and save the results in a JSON file, and return the results in the terminal

## if you run into an error for level1 scraping:
you can see what the computer is doing by going here:
```python
# if you want to see the browser, set headless=False -- >ctrl + shift + f this comment, its in level1_scraper.py, line 52
browser = p.chromium.launch(headless=True)
```
## for future Ali AND if you are getting errors:
For some reason it is working fine with python 3.9.13, idk why, but it is.
But if not:
Make sure your python version is 3.11 or higher, but *DONT GET* 3.13. The ScrapeGraph API is not compatible with 3.13.
if you need to downgrade your python version, you can do it here: https://www.python.org/downloads/
check your python version by running this in command prompt HAVE YOUR VIRTUAL ENV ACTIVATED:
```python
python --version
```
