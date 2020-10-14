This is a dotnetcode console app (create with dotnet new console) modified to add Kestrel.

Steps to run Locally:

dotnet restore
dotnet run
<browse to localhost:5000>


Steps to run in Container

dotnet restore
docker build . -t dotnetcoreimage:1.0
docker push dotnetcoreimage:1.0
docker run -it -p 5000:80 dotnetcoreimage:1.0
<browse to localhost:5000>
