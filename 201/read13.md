# Local Storage

### Web storageprovides web apps with methods and protocols for storing client-side data. Web storage supports persistent data storage, similar to cookies but with a greatly enhanced capacity and no information stored in the HTTP request heade

### The localStorage and sessionStorage properties allow to save key/value pairs in a web browser. The localStorage object stores data with no expiration date.


### The localStorage object stores data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.

### Also look at the sessionStorage property which stores data for one session (data is lost when the browser tab is closed).

### The localStorage property is read-only.

### The Web Storage API defines two types of storage areas ― local storage and session storage. Local storage is persistent data which remains until it is explicitly deleted, or until the browser's cache is cleared. According to the specification, browsers should allocate at least 5MB of local storage per domain

### The storage belongs to the user so the user can clear it if they want to. ... You should think of LocalStorage as a long term cache that usually will remain with that particular browser on that particular computer, but will not always be there.


## Syntax
### * ` window.localStorage `
### *  `localStorage.setItem("key", "value");`
### * ` lvar lastname = localStorage.getItem("key");`
### * `localStorage.removeItem("key");`







## resources :


* w3schools
* http://diveinto.html5doctor.com/storage.html
* https://www.sitepoint.com/an-overview-of-the-web-storage-api/
* https://stackoverflow.com/questions/9728946/localstorage-data-persistence
