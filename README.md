# Example Application - Complimentr

This application is meant to be used with the [Introduction to APIs course](https://github.com/craigsdennis/intro-to-apis-course).

## Use this on Glitch

[Remix on Glitch](https://glitch.com/edit/#!/import/git?url=https://github.com/craigsdennis/intro-to-apis-flask)

⚠️ Several students have reported that cloning erroneously sets up a default Glitch application. If this happens to you, in the Glitch app that is created choose **Tools** >> **Extras** >> **Git Import and Export** >> **Import from GitHub** when prompted enter  `craigsdennis/intro-to-apis-flask`

## Local Installation

Copy `.env.example` to `.env` and update it with your [Twilio](https://twilio.com) credentials.

### Running the application

* `python -m venv .venv`
* `source ./.venv/bin/activate`
* `pip install -r requirements.txt`
* `FLASK_ENV=development flask run`

#### In Development mode

* Run [ngrok](https://ngrok.com/) on port 5000
* Visit your ngrok url!

### Hiding the car keys

Creating the `client` object: 
* `client = Client()`

Not passing any arguments to the `client` object on creation causes the object to look at your environment variables (e.g., `.env`) for those variables. 

**PROTIP:** Environment variables are an excellent way to keep your keys hidden -- and not leaving them on the front seat. Check the notes for how to do this locally on your machine.
