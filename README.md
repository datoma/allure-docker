# Dockerized Allure2

This is wrapper around [Allure](https://docs.qameta.io/allure/). You can use it like Allure installed on your local machine.

Generating report:

```
docker run -v `pwd`/allure-results:/app/allure-results -v `pwd`/allure-report:/app/allure-report imanel/allure generate --clean
```

Starting server:

```
docker run -v `pwd`/allure-results:/app/allure-results -v `pwd`/allure-report:/app/allure-report -p 8080:8080 imanel/allure serve -p 8080
```

## cloned from 
https://github.com/imanel/allure-docker/blob/master/README.md

## License

(The MIT License)

Copyright © 2020 Bernard Potocki

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ‘Software’), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
