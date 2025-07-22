FROM rust:1.85.1

WORKDIR /app

RUN cargo install cargo-watch

EXPOSE 8000

COPY ../app .

CMD ["cargo", "watch", "--poll", "-x", "run"]
