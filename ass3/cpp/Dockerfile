FROM gcc:latest

RUN apt-get update && apt-get install -y cmake
COPY . /home/bentau/myapp
WORKDIR /home/bentau/myapp

RUN mkdir build
WORKDIR /home/bentau/myapp/build

RUN cmake .. && make


CMD [ "./runTests" ]