import requests
import json
import urllib

def login(username, password):
    
    parameters = {
        'username': username,
        'password': password,
        'client_id': 'OAuthPage',
        'redirect_uri': '/main/',
        'scope': '',
        'state': '4E252A',
        'response_type': 'code',
        'tenant': 'tabor'
        }

    #Start a Session.
    session = requests.Session()
    open_url = session.post('https://tabor.zportal.nl/api/v2/oauth', data = parameters, allow_redirects = True)

    print('[SYSTEM] Status code ', open_url.status_code)
    print(open_url.text)


