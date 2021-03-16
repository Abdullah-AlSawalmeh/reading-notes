In order to manage data handled by your web application, you do not necessarily need a database. The respective Browser Storage features are supported by Chrome (version 4 and higher), Mozilla Firefox (version 3.5 and higher) and Internet Explorer (version 8 and higher), and a range of other browsers including those of iOS and Android.

# localStorage
Any content/data saved to the localStorage object will be available after the browser has been restarted (closed and opened again). In order to save an item to localStorage, you can use the method setItem(). This method must be handed a key and a value.

```
Example: localStorage.setItem("mykey","myvalue");
```
To retrieve the item from the localStorage, the method getItem must be used. The getItem method must be handed the key of the data you would like to retrieve:

```
  Example: localStorage.getItem("mykey");
  ```

  Saving arrays to localStorage and sessionStorage
You cannot just save single values to the localStorage and sessionStorage, but you can also save the content of an array.

In order to be saved, the array must first be converted to a string. In the example shown above, we are using the JSON.stringify method to accomplish this.

When retrieving our data from the localStorage or sessionStorage, convert it back to an array:
