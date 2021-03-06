## List of HTTP status codes

## How to install

Just run

```shell
npm install http-status-codes-js
```

add the `--save` option to add it to the `dependencies` in your `package.json` as well

## How to use

Import the module

```ecmascript 6
import httpStatusCodes from 'http-status-codes-js';
```

Find the status code you are interested in among `INFORMATION`
, `SUCCESS`, `REDIRECTION`, `CLIENT_ERRORS` and `SERVER_ERRORS` and use
it in your request.

```ecmascript 6
router.get('/', function(req, res, next) {
  res.status(httpStatusCodes.SUCCESS.OK);
  
  // Do something
});

```

# About

The module was created as simple way of avoiding using `magic numbers`
in the source code to represent the `http statuses` and improve
api readability.

I also hope that it's going to be a good reference for all of us
to go beyond the standard usages of `http status codes` and create
better and more descriptive `API's`.