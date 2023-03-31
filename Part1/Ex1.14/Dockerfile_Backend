FROM golang

EXPOSE 8000

WORKDIR /usr/scr/app

COPY . .

RUN go build

ENV PORT=8000
ENV REQUEST_ORIGIN=http://localhost:5000

CMD ["./server"]