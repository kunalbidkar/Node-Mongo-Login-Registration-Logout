# Node-Mongo-Login-Registration-Logout
This app is made using node.js, mLab, to implement user login, registration and logout feature
Entry point of the application is app.js

## Configuration
You can change your DB_URL inside app.js with your custom mLab mongodb path. 
Note: kunalbidkar is the user created inside my schema and password1 is the password for that specific user. 
kloudio is the name of my schema.

```
if (app.get('env') != 'live'){
	process.env.DB_URL = 'mongodb://kunalbidkar:password1@ds153495.mlab.com:53495/kloudio';
}	else {
// prepend url with authentication credentials // 
	process.env.DB_URL = 'mongodb://kunalbidkar:password1@ds153495.mlab.com:53495/kloudio';
}

```

If you wish to add or remove any country in the form then you can configure that in app/server/modules/country-list.js

## Usage
Clone this project and run these commands in the root folder

```
npm install
npm start
```


After the npm start command, the app starts the server. Once the server is started, open<br>
your browser at [http://localhost:3000](http://localhost:3000).

