# blog-post-server

An JSON database for the [BlogPost](https://github.com/memonsahil/BlogPost) app.

## Setup

1. Install the project using [npm](https://www.npmjs.com/get-npm):
````
$ npm install
````

2. Install its dependencies - [json-server](https://github.com/typicode/json-server) and [ngrok](https://github.com/bubenshchykov/ngrok) globally on your system:
````
$ npm install -g json-server ngrok
````

3. Launch the database:
````
$ json-server -w db.json
````

4. Run the ngrok server:
````
$ ngrok http 3000
````

5. Replace the baseURL for the [API](https://github.com/memonsahil/BlogPost/blob/master/src/api/jsonServer.js) in the BlogPost project with the ngrok forwarded URL. Note that the ngrok forwarded URL changes every 8 hours.

6. After completing the above steps, the BlogPost app will connect to the JSON database on launch.

## Contributing
Pull requests are welcome. For major changes, please open an issue first.

## License
MIT &copy; [memonsahil](https://github.com/memonsahil)
