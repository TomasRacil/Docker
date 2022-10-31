FROM node

WORKDIR /usr/src/frontend

ENV BACKEND_URL=backend
ENV BACKEND_PORT=5000

# install app dependencies
COPY /app/ .
#WORKDIR /usr/src/frontend/app
RUN npm install 
RUN npm install react-scripts@3.4.1 -g 
RUN npm install -g serve

# add app

#COPY /app/build/ .

#CMD ["npm", "start","80"]
CMD ["serve", "-l", "80"]