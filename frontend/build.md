# to build front end image

#### update front end source code
git submodule update --remote

#### build front end dist
cd clickboard-fe
npm install
npm run build

#### build docker image
cd ..
docker build -t keynezzz/clickboard-fe .
