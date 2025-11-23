FROM ubuntu

WORKDIR /app

RUN apt-get update && apt-get install -y dos2unix curl

COPY script.sh .

RUN dos2unix script.sh
RUN chmod +x script.sh

CMD ["./script.sh"]
