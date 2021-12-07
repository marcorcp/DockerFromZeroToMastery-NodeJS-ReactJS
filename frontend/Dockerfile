FROM node:12.16.2
WORKDIR /app
COPY ["package-lock.json", "package.json", "./"] 
RUN npm install --production
COPY . . 
EXPOSE 80
CMD ["npm", "start"]
