# golang-backend-boilerplate

This repo serves as a boilerplate project for golang web applications.

The project starter is **NOT** a web framework in any sense. Instead, it still relies on golang standard library to build web applications. Community packages are added as needed.

## System Requirements

* [Golang](https://golang.org/)
* (Optional) [PostgreSQL](https://www.postgresql.org/)

If you don't want PostgreSQL as your database solution, you may remove PostgreSQL related code from this boilerplate project by yourself.

## Technology Stacks

Packages used in this boilerplate project:

* [joho/godotenv](https://github.com/joho/godotenv)
* [sirupsen/logrus](https://github.com/sirupsen/logrus)
* [urfave/negroni](https://github.com/urfave/negroni)
* [julienschmidt/httprouter](https://github.com/julienschmidt/httprouter)
* [rs/cors](https://github.com/rs/cors)
* [jinzhu/gorm](https://github.com/jinzhu/gorm)
* [lib/pq](https://github.com/lib/pq)

## Usage

### Initiate a New Backend Project

Clone this repo with `git`:

```
$ git clone https://github.com/cwchentw/golang-backend-boilerplate.git
$ mv golang-backend-boilerplate myapp
$ cd myapp
```

You should always reset the path to remote repo for your own web application:

```
$ git remote set-url origin path/to/remote/repo
```

### Install dependencies

On Unix-like OSes, run this shell script to install dependencies:

```
$ ./install.sh
```

On Windows, run this batch script instead:

```
$ .\install.bat
```

### Prepare a PostgreSQL database

This boilerplate project chooses PostgreSQL as its database. Therefore, you should prepare your own database first.

Alternatively, you may delete PostgreSQL related code in this project, replacing it with the code related to your own database solution.

### Set Environment Variables

If you keep the PostgreSQL related code in your project, you should set five database related environment variables:

* **DB_HOST**
* **DB_PORT**
* **DB_USER**
* **DB_NAME**
* **DB_PASS**

You may set these variables either on a private *.env* file or on your own system. The *.env* file should not be committed to your project.

### Time to Hack

Begin to build next awesome web application.

## Copyright

2019, Michael. This repo itself is licensed under [MIT license](https://opensource.org/licenses/MIT). Nevertheless, you may adopt it in your own project with any license you prefer.
