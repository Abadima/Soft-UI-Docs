# Database Driver
Starting from 1.5.0-beta.1, you are able to use database drivers! This means you can use MongoDB, MySQL, etc for your storage needs. This will store everything that needs to be persistent. (Feeds are stored seperately)

## Database Driver Options
Because we use Keyv you are able to set your database driver to anything Keyv supports.

The list of options are at https://www.npmjs.com/package/keyv but we will provide the two most common ones on this guide.


## Defaults
The default storage adapter (the type of storage) is SQLite which will store your data in a file, if you use Git then this file will most likely be overwritten when you make an update to your files.

## Setting a Database Driver
To set a database driver, add this bit of code to the theme config.
```js
dbdriver: "your dbdriver"
```

## MongoDB
To add a driver like MongoDB you need to install the adapter with this command.
```js
npm install --save @keyv/mongo
```
And then set the driver to your connection string such as this.
```js
mongodb://user:pass@localhost:27017/dbname
```

## MySQL
To add a driver like MySQL you need to install the adapter with this command.
```js
npm install --save @keyv/mysql
```
And then set the driver to your connection string such as this.
```js
mysql://user:pass@localhost:3306/dbname
```