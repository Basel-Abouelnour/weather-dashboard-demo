# Weather Dashboard Demo
this is a weather app written in python in the 30-day-devops-challenge #DevOpsAllStarsChallenge

---

## Project Structure
```
.
|-- README.md
|-- data
|-- requirements.txt
|-- src
|   |-- __init__.py
|   `-- weather-dashboard.py
`-- tests

3 directories, 4 files
```
---
## Functions
### Create AWS S3 bucket 
- First it checks if the bucket name already exists on your AWS account, if it does it proceed to the next function
- If the S3 bucket name doesn't exist on your account it creates it

### Fetch Weather 
- It fetches the weather data for the Cities selected in the code in a json format to be showed later in the terminal

### Saving Data to the S3 Bucket
- After finishing fetching the data, it saves it to the S3 bucket we created before each as an object with the timestamp for each city

---

## Output sample
- this is an ouput sample for two cities Beni Suef and Cairo :-
```
$ python src/weather-dashboard.py

Bucket weather-dashboard-24462 exists
Successfully created bucket weather-dashboard-24462

Fetching weather for Beni Suef...
Temperature: 21.92°C
Feels like: 21.03°C
Humidity: 33%
Conditions: overcast clouds
Successfully saved data for Beni Suef to S3
Weather data for Beni Suef saved to S3!

Fetching weather for Cairo...
Temperature: 20.42°C
Feels like: 19.69°C
Humidity: 45%
Conditions: scattered clouds
Successfully saved data for Cairo to S3
Weather data for Cairo saved to S3!
```
