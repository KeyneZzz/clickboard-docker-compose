# ClickBoard
Quickly copy one of many saved strings by a single click. No need to move your finger between C and V very often.

## Something You Should Know Before Start
1. Clicking save button will save all the content, although it has save button on every line.
2. No auth in this service. If you need one, you can proxy it with Nginx and Authelia.
3. The backend save the data as a plaintext json file, which can never be safe. If you want to save some really important key/passwd/token, DO NOT USE THIS SERVICE.

## Deploy
1. `git clone https://github.com/KeyneZzz/clickboard-docker-compose.git`
2. in `docker-compose.yml` change 8080 to whatever port you would like to deploy
3. `docker-compose up -d`
