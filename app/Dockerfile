# path: ./Dockerfile

FROM node:16-alpine as development

# Installing libvips-dev for sharp Compatibility
RUN apk update && apk add --no-cache build-base gcc autoconf automake zlib-dev libpng-dev nasm bash vips-dev

RUN npm config get registry

RUN npm install -g strapi

RUN mkdir /usr/app

WORKDIR /usr/app

CMD ["./start.sh"]
