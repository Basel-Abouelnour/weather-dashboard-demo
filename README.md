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
