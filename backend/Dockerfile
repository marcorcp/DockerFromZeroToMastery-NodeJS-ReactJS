FROM node:12.16.2
WORKDIR /app
COPY ["package-lock.json", "package.json", "wait-for.sh", "startup.sh", "./"] 
RUN apt-get update  && apt-get install netcat -y && chmod +x ./wait-for.sh ./startup.sh && npm install --production
COPY . . 
EXPOSE 5000
CMD ["npm", "start"]
