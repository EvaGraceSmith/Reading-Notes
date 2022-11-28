## Reading

### [Local Storage and How To Use It On Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

#### Why would a developer use local storage for a web application?
* The main problem with HTTP as the main transport layer of the Web is that it is stateless. This means that when you use an application and then close it, its state will be reset the next time you open it. If you close an application on your desktop and re-open it, its most recent state is restored.
This is where local storage comes in. You would keep a key on the user’s computer and read it out when the user returns.


#### What information should not be stored in local storage?
We shouldn't  record user actions and information without the user’s knowledge.


#### Local storage can store what type of data? 
strings

#### How would you convert it to that type before storing?
By using the native JSON.stringify() and JSON.parse() methods:
var car = {};
car.wheels = 4;
car.doors = 2;
car.sound = 'vroom';
car.name = 'Lightning McQueen';
console.log( car );
localStorage.setItem( 'car', JSON.stringify(car) );
console.log( JSON.parse( localStorage.getItem( 'car' ) ) );

## Bookmark/Skim

### [“The Past, Present, and Future of Local Storage for Web Applications”](http://diveinto.html5doctor.com/storage.html)

Cookies can be slow, unencrypted and low data

What we really want is

* a lot of storage space
* on the client
* that persists beyond a page refresh
* and isn’t transmitted to the server


provides code for using local storage from hTML5
