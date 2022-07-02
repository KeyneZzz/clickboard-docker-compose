# ClickBoard
Quickly copy one of many saved strings by a single click. No need to move your finger between C and V very often.

![Kapture 2022-07-03 at 00 34 13](https://user-images.githubusercontent.com/6895745/177008963-587f7f2c-4a2b-470c-beec-c9282664b1b6.gif)

## Something You Should Know Before Start
1. Clicking save button will save all the content, although it has save button on every line. (Add/delete line will save all too)
2. No auth in this service. If you need one, you can proxy it with Nginx and Authelia.
3. The backend save the data as a plaintext json file(backend/clipboardObjects.json by default), which can never be safe. If you want to save some really important key/passwd/token, DO NOT USE THIS SERVICE.

## Deploy
1. `git clone https://github.com/KeyneZzz/clickboard-docker-compose.git`
2. in `docker-compose.yml` change 8080 to whatever port you would like to deploy
3. `docker-compose up -d`
