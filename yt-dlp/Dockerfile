FROM ubuntu:24.04

WORKDIR /mydir

RUN apt-get update && apt-get install -y curl python3 ffmpeg

RUN curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp
RUN chmod a+x /usr/local/bin/yt-dlp

ENTRYPOINT ["/usr/local/bin/yt-dlp"]

CMD ["https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.newyorker.com%2Fnews%2Fdaily-comment%2Fmonkey-see-monkey-click&psig=AOvVaw1B4aaZfYWfPiuIlKEhDntW&ust=1764076048642000&source=images&cd=vfe&opi=89978449&ved=0CBUQjRxqFwoTCNjT48PtipEDFQAAAAAdAAAAABAE"]

