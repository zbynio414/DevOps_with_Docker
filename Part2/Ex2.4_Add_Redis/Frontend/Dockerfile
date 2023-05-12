FROM node:16.20.0-alpine

EXPOSE 5000

WORKDIR /usr/src/app


COPY package* .

#install dependecies
RUN npm install

#install serve
RUN npm install -g serve

COPY . .
#build static
RUN REACT_APP_BACKEND_URL=http://localhost:8000 npm run build

CMD ["serve", "-s", "-l", "5000", "build"]
