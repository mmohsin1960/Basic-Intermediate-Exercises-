
#FROM golang:1.8    (first Edit)

FROM golang:alpine AS builder

WORKDIR /firstapp

COPY firstapp.go . 

RUN go mod init firstapp 

 
RUN go build -o appexecuteable .




#========= After write above "AS builder"
FROM alpine

WORKDIR /app

COPY --from=builder /firstapp/ /app/

CMD  ["./appexecuteable"]


