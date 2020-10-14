This is a dotnetcode console app (create with dotnet new console) modified to add Kestrel.

**Steps to run Locally:**

dotnet restore<br>
dotnet run<br>
*browse to localhost:5000*


**Steps to run in Container**

dotnet restore<br>
docker build . -t dotnetcoreimage:1.0<br>
docker push dotnetcoreimage:1.0<br>
docker run -it -p 5000:80 dotnetcoreimage:1.0<br>
*browse to localhost:5000*<br>
