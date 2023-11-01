# api-endpoint-finder
This repo is for a Python script that parses an HTML page and identifies API endpoints and their HTTP methods to use for software testing.

## Requirements

This script requires the following libraries:

- requests
- bs4
- termcolor
These can be installed using pip:

```bash
pip install requests bs4 termcolor

```

## Usage

- Set the target URL by changing the url variable in the script.
- Run the script using python api_endpoint_finder.py.
- The script will output the API endpoints and their HTTP methods.


## Sample Output

```bash
GET https://api.example.com/v1/users
Payload: {}

POST https://api.example.com/v1/users/new
Payload: {'username': 'johndoe', 'password': 'password'}

GET https://api.example.com/v1/users/1
Payload: {}

PUT https://api.example.com/v1/users/1
Payload: {'username': 'johndoe', 'password': 'newpassword'}

DELETE https://api.example.com/v1/users/1
Payload: {}

PATCH https://api.example.com/v1/users/1
Payload: {'username': 'johndoe'}

HEAD https://api.example.com/v1/users
Payload: {}


```
## The HTTP methods are color-coded as follows:

GET: #0f6ab4

POST: #10a54a

PUT: #c5862b

DELETE: #a41e22

PATCH: #D38042

HEAD: #ffd20f


