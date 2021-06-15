# blog-post-server

![Maintenance](https://img.shields.io/badge/Maintained%3F-no-red.svg)
![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)
![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)

A JSON database for the [Blog Post](https://github.com/memonsahil/blog-post) app.

## Setup

1. Install the project using npm:

````
$ cd blog-post-server && npm install
````

2. Install [json-server](https://github.com/typicode/json-server) globally to initiate a local JSON database:

````
$ npm install -g json-server json-server
````

3. Install [ngrok](https://github.com/bubenshchykov/ngrok) globally to create a proxy URL for the JSON database:

````
$ npm install -g ngrok
````

4. Launch the JSON database:

````
$ npm run db
````

5. Launch the ngrok server:

````
$ npm run tunnel
````

6. Replace the baseURL in the [API](https://github.com/memonsahil/BlogPost/blob/master/src/api/jsonServer.js) within the blog-post project with the ngrok forwarded URL.

After completing the above steps, the Blog Post app will connect to the JSON database on launch.

## Contributing

Pull requests are welcome. For major changes, please open an issue first.

## License

MIT &copy; [memonsahil](https://github.com/memonsahil)
