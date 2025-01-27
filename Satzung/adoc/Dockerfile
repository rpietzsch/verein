FROM asciidoctor/docker-asciidoctor:main

RUN apk update && apk add go-task ghostscript
RUN ln -s /usr/bin/go-task /usr/bin/task

# https://github.com/github/pages-gem/issues/839
RUN apk add gcompat
RUN gem install nokogiri

RUN mkdir /data
WORKDIR /data