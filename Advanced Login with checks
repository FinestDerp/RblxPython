print("content-type: text\html\n" )
import requests
import os
import json

def newLogin(username, password):
    session = requests.Session()
    login = session.post('https://www.roblox.com/newlogin', data = {'Username':username,'Password':password}).text
    if 'Your username or password is incorrect. Please check them and try again.' in login:
        print('Incorrect')
	elif 'We need to make sure you' in login:
		print('Captcha')
    else:
        print('Correct')
        session.close()

newLogin("USER","PASS")
