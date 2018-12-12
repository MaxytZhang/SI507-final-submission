# Douban Top250 VS IMDB Top250
### version 1.0

## Project Description
A web application based on Flask, Sqlite, HTML5/Bootstrap, JavaScript, supports
information comparison between people's views of Top250 movies in Douban and in IMDB.<br>
*Douban is a Chinese version of IMDB and it's really popular among movie fans<br>*

## Supported Functions
Search movies based on their ranks in Douban Top250<br>
Compare their ranks, rating, votes between Douban and IMDB<br>
Display the wordcloud for actors<br>
Display the wordcloud for director<br>
Display the weight of different genres<br>

## Data Sources
IMDB data: OMDB API<br>
Douban data: https://movie.douban.com/top250<br>
*requests is used to fetch the data from website<br>*
*prepare your OMDB API KEY!*

## Get Started
*Please follow the instructions to guarantee data is ready<br>*
*requirement.txt includes all the libraries required<br>*

### Virtual Environment

```
$ pip3 install virtualenv
$ virtualenv venv
$ source venv/bin/activate
(venv) $ pip install -r /path/to/requirements.txt 
```
If you want to close the virtual environment<br>
```
$ Deactivate
```

### API KEY
You apply your OMDB API KEY here:<br>
http://www.omdbapi.com/apikey.aspx<br>
Create a python file named **secret.py**<br>
And enter your API KEY!
```
api_key = 'your_api_key'
``` 

### Data Sample
You can directly use the data sample provided by downloading **douban_cache.json, imdbb_cache.json, movie.dbb**<br>
*In this way, you don't need to do the data collection part*

### Data Collection
```
(venv) $ python data.py
```
Once you see ***You have successfully build the databse!*** you can continue<br>
*It may take some time to fetch all the data for the first time. Be patient!*


### Test
```
(venv) $ python main_test.py
```
Pass the test to guarantee you collect the right data

### Run the App
```
(venv) $ python app.py
```
*you can quit it by pressing CTRL+C*

### Website Address
http://127.0.0.1:5000/<br>

## Author
**Max Zhang**<br>
https://github.com/MaxytZhang/507-final-project