# Class 13 - Local Storage

## [Article](http://diveinto.html5doctor.com/storage.html): The Past, Present, and Future of Local Storage for Web Applications

- Cookies were invented early in web history and can be used for local storage but there is downsides, they can slow down your web application and they are limited in size.
- Internet Exlorer introduced userData, allowing web pages to store up to 64kb of data per domain in xml.
- Other solutions were presented before HTML5 but they were either specific to a browser or reliant on a third-party plugin.
- HTML5 created localStorage objects which are supported accross browsers and save the data even when you leave the page. It does not use cookies. It does not have to rely on a backend server.
- HTML5 storage is based on key:value pairs, all datatypes are supported but it is actually stored as a string so you will need to parse retrieved data.
- Calling getItem() on a non-existent key will return null rather than throw an exception
- Accessing you can use getItem/setItem or square bracket notation on localStorage object simply called `localStorage`.
- Can also call a value by key() or removeItem()
- Can add storage to an event listener with "storage"
- Storage event object contains information including key, oldValue, newValue and url (the page that called a method that triggered this change)
- Limitation: 5mb storage per domain (storage quota) and you cannot ask the user for more storage space.
- The future is undecided, it might include a sql database in the form of WebDB or something else.

[<== Back](../README.md)
