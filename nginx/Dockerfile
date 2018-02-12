FROM ubuntu:16.04

RUN apt-get update && apt-get install -y nginx curl

COPY nginx.conf /etc/nginx/nginx.conf
COPY nginx-app.conf /etc/nginx/sites-available/default

CMD ["nginx", "-g", "daemon off;"]
