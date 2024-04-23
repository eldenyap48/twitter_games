# Twitter Games
- Play "Who Said That" and "Higher or Lower" with our game built using the X Api!
- [Click here for a video demonstration](https://youtu.be/BKOgVMVG_uI)

## Introduction
- Engage with your favorite celebrities through games like "Who Said That" and "Higher or Lower" generated using real tweets pulled from the X api!!
- Stay up-to-date with their latest post, and explore more celebrities
- Have fun!!

---

## Requirements
- You must have a Twitter development account with approval for the Academic Research Product Track to play this game
- You need to have a ngrok account, or any web hosting service, to run this app

## Steps to run the program
### Frontend
- `npm install`
- `npm start`

### Backend
- Create a new environment
- `pip install -r requirements.txt`
- Go to your twitter development account, and copy the bearer token, consumer and consumer secret keys into the app.py file
- `flask run`
- Expose your localhost endpoint to the web using ngrok by running `ngrok http <replace with your endpoint>`
- Go to the twitter development account, replace the callback URI under app settings with the ngrok endpoint
- Replace the callback url in the app.py file with your `<your ngrok endpoint>/callback`
- In the frontend, replace all instances of the api call in the frontend with your ngrok endpoint, or your sessions won't work
