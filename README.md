# install-appMo-netPro
เตรียมตัวก่อนเขียน Code

ติดตั้ง Sublime Text 3
```
$ sudo add-apt-repository -y ppa:webupd8team/sublime-text-3
$ sudo apt-get update
$ sudo apt-get install sublime-text-installer
```
ลง packet 
Ctrl+` 
```
import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```
Ctrl+Shift+P
```
Install Packet
Emmet
```

ติดตั้ง nodeJS
```
$ sudo apt-get update && sudo apt-get install -y build-essential openssl libssl-dev pkg-config
$ wget -c "http://nodejs.org/dist/v0.12.0/node-v0.12.0.tar.gz"
$ sudo tar -xzvf node-v0.12.0.tar.gz
```

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
