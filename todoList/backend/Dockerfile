FROM golang
RUN mkdir /backend
ADD . /backend
WORKDIR /backend
RUN go get -d github.com/gorilla/mux
RUN go get -d github.com/go-sql-driver/mysql
RUN go get -d github.com/jinzhu/gorm
RUN go get -d github.com/rs/cors
RUN go get -d github.com/sirupsen/logrus
RUN go build
CMD ["go", "run", "backend.go"]