FROM node:latest

RUN mkdir -p  /parse



WORKDIR /parse

COPY . /parse

RUN npm install

ENV APP_ID "0742vWqaHDnW5VkvbTogyh2O9UbdXDlAe19XOPd2Tc"
ENV MASTER_KEY "La7U4b8Hxdsu2kwcV6ou08JWGlCdCETjkyR9H8DIXw"
ENV DATABASE_URI "mongodb://mongo:27017/my-db"

# Optional (default : 'parse/cloud/main.js')
# ENV CLOUD_CODE_MAIN cloudCodePath

# Optional (default : '/parse')
# ENV PARSE_MOUNT mountPath

EXPOSE 1337

# Uncomment if you want to access cloud code outside of your container
# A main.js file must be present, if not Parse will not start

VOLUME /parse/cloud               
