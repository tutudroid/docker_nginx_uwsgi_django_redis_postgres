FROM my_ubuntu 

RUN mkdir -p /my_web

WORKDIR /my_web

COPY ./ /my_web

CMD ["uwsgi", "--ini", "uwsgi.ini"]
