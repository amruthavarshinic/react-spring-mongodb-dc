### Setup React-spring-mongodb Employees demo app

Open a terminal and run below command to start frontend
```sh
cd frontend-react
npm start
```
Open another termal and run below command fro up and running backend

```sh
cd backend-springboot
mvn -c spring-boot:run
```
Install mongoDB using docker
```sh
docker run -d -p 27017:27017 --name my-mongodb mongo
```
### Install insomnia and inso cli

```sh
# Add to sources
echo "deb [trusted=yes arch=amd64] https://download.konghq.com/insomnia-ubuntu/ default all" \
    | sudo tee -a /etc/apt/sources.list.d/insomnia.list

# Refresh repository sources and install Insomnia
sudo apt-get update
sudo apt-get install insomnia

# download the Linux tar file
wget https://github.com/Kong/insomnia/releases/download/lib%408.5.1/inso-linux-8.5.1.tar.xz

# Extract the file
tar -xf inso-linux-8.5.1.tar.xz

# check inso cli version
./inso --version
```

- Add employee-spec.yaml to insomnia Document
