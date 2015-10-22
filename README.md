# install-appMo-netPro
เตรียมตัวก่อนเขียน Code

ติดตั้ง Sublime Text 3
```
$ sudo add-apt-repository -y ppa:webupd8team/sublime-text-3
$ sudo apt-get update
$ sudo apt-get install sublime-text-installer
```
ติดตั้ง nodeJS
'''
$ curl -sL https://deb.nodesource.com/setup | sudo bash -
$ sudo apt-get install nodejs
$ sudo apt-get install npm
$ sudo ln -s /usr/bin/nodejs /usr/bin/node
'''
Mongoose
Download
```
$ git clone https://github.com/divHacker/homework-api-mongoose.git
$ cd homework-api-mongoose
$ npm install
```

Start Mongodb
```
$ mongod --dbpath ./data
```

Start App
```
$ nodemon index.js
```

POST -> http://domain/api/homework
GET -> http://domain/api/homework

JSON
```
{
	ip_addr: String,
	port: number,
	name: String
}
```
