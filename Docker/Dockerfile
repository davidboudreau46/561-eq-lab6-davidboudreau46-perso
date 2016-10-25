FROM ymazieres/dotnet:compile
WORKDIR /src
EXPOSE 5000
ENV ASPNETCORE_URLS http://+:5000

CMD ["sh", "/script/run.sh"]
COPY /Docker/run.sh /script/run.sh
RUN chmod +x /script/run.sh

COPY /src /src

#docker build -t webapp -f ./Docker/DockerFile . 

#docker run -it --rm -v $PWN/packages:/root/.nuget/packages -p 8080:5000 webapp:test

#docker run -it --rm -v $PWD/packages:/root/.nuget/packages webapp:test