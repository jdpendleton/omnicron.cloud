<h1 align="center">
<img src="assets/icon.png" alt="Icon" width="200" height="200" </img>
<br>omnicron.cloud<br>
</h1>

**What Is This?** - Allows you to Run any HTTP request type at a Unix cron interval between a start date and an end date

## Features
- Authenticate to the Omnicron API using Google authentication to obtain a token
- Commission an Omnicron job with a POST request
- Enable or disable an Omnicron job with a PATCH request
- Decommission an Omnicron job with a DELETE request
- Access your Omnicron jobs with a GET request
- Access your job execution response objects with a GET request

## Purpose
Schedule any code to run, any time, anywhere, on any schedule.

## Usage
url: https://api.omnicron.cloud/v1/

### /token
post your google credentials to retrieve a token

### /jobs
</br>

GET  
query your omnicron jobs  
</br>

POST  
create an omnicron job
```json
{
    "start_date": "2022-02-28",
    "end_date": "2022-03-31",
    "cron": "* * * * *",
    "request_type": "POST",
    "request_url": "https://api.mysite.com/v1/sendtextmessage",
    "request_headers": "{}",
    "request_data": "{'number': '13179792681', 'message': 'hello, world!'}",
}
```

### /runs
</br>

GET  
query your omnicron runs  
</br>

## Contact info 
Submit issues [here](https://github.com/jdpendleton/omnicron.cloud/issues), email jdpendleton@alumni.fullsail.edu for questions

## License
[GNU GENERAL PUBLIC LICENSE](LICENSE)