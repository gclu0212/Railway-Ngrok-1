# Railway-Ngrok
Using Ngrok to penetrate Railway Docker's internal network to use ubuntu

## 1/ Register for a railway & ngrok . account

* First you need to have a github account. Register [here](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) if not already
1. Access [Railway](https://railway.app/login) Visit the website to register for a Railway account and log in directly with your github account
2. Access [Ngrok](https://dashboard.ngrok.com/auth) Go to the website, and sign up for a free account
3. Access [Ngrok Authtoken](https://dashboard.ngrok.com/auth) copy and save your `Authtoken` code

Notes: A region's Ngrok free account can only have one tunnel service, so if you want to deploy multiple projects, please modify the region

## 2/ Implementation

Click the button below to deploy

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https://github.com/milan-says/Railway-Ngrok&envs=NGROK_TOKEN,PASSWORD,PORT,REGION&PASSWORDDesc=M%E1%BA%ADt%20kh%E1%BA%A9u%20d%C3%B9ng%20%C4%91%E1%BB%83%20%C4%91%C4%83ng%20nh%E1%BA%ADp%20ssh%20%28do%20b%E1%BA%A1n%20t%C3%B9y%20ch%E1%BB%8Dn%29&NGROK_TOKENDesc=Authtoken%20%C4%91%C3%A3%20%C4%91%C4%83ng%20k%C3%BD%20trong%20ngrok&PORTDesc=Open%20port%20you%20need%2C%20default%20is%2080&PORTDefault=80&REGIONDesc=Khu%20v%E1%BB%B1c%20ngrok%2C%20m%E1%BA%B7c%20%C4%91%E1%BB%8Bnh%20l%C3%A0%20jp%2C%20t%C3%B9y%20ch%E1%BB%8Dn%20us%2Feu%2Fap%2Fau%2Fsa%2Fjp%2Fin&REGIONDefault=jp&referralCode=IGBnmG)

`PASSWORD`: Fill in the password for ssh login (your choice)

`NGROK_TOKEN`: Enter `Authtoken` registered in `Ngrok`

`PORT`: Fill in the port (PORT) you created the app and Railway will automatically forward it to the domain name given to you, default: 80

`REGION`: Fill in the area with tunnel service, as close as possible, default is jp, optionally us/eu/ap/au/sa/jp/in

## 3/ Note
All data will be deleted if you restart the railway project
