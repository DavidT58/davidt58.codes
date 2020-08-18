# My experimental website

This main purpose of this website is to test and deploy various web technologies - basically a playground.

## General information

This [website](https://davidt58.codes) is currently deployed on digital ocean, on a single Ubuntu 18 droplet.

Currently, I am testing an URL shortener implemented in NodeJS + Express, along with a MongoDB database for storing shortened URL's.

The front-end needs more work, but the back-end works as exprected;

## Usage

Alternatively, you can clone this repo and run the website locally with the following commands:

```bash
cd davidt58.codes/server
npm install
npm run dev
```

POST and GET are implemented, so simply if you type davidt58.codes/helloworld (GET method) in your web browser it will lead you to helloworld.rs

Similarly, if you make a POST query with a custom slug, it will put in the database and you could access it;

JSON format for the POST query: 
{
  "slug": "string",
  "url": "url of the website to be shortened"
}

In case the slug is not provided it will be automatically generated

### Requirements:
NodeJS v12

MongoDB v3.6.3

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## License
[MIT](https://choosealicense.com/licenses/mit/)
