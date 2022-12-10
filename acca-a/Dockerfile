FROM node:alpine
RUN apk add --no-cache curl

## Web port variable to run the application
ENV WEB_PORT=3002

## Docker expose port value
EXPOSE 3002


## Working Directories 
WORKDIR /app
ADD . /app


## Installing packages and make build for tsc to node
RUN yarn install && yarn build


##Running application
CMD ["yarn", "start"]

