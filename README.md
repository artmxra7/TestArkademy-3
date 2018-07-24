# Arkademy 3 Test


Berikut adalah jawaban dari soal seleksi arkademy bootcamp #3

## Soal Nomor 1 s/d 5

Directory Soal 1 - 5 :

* [soal 1 s/d 5](https://github.com/artmxra7/TestArkademy-3/tree/master/Soal1-5) - Menggunakan javascript;

### package.json

```
{
  "name": "arkademy-test",
  "version": "1.0.0",
  "description": "Jawaban dari soal test bootcamp arkademy#3",
  "scripts": {
    "soal-1": "node soal-1.js",
    "soal-2": "node soal-2.js",
    "soal-3": "node soal-3.js",
    "soal-4": "node soal-4.js",
    "soal-5": "node soal-5.js",
    "soal-6": "node soal-6.js",
    "soal-7": "node soal-7.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
   "keywords": [
    "testarkademy3"
  ],
  "repository": {
    "type": "git",
    "url": "git+https://github.com/artmxra7/TestArkademy-3.git"
  },
   "author": "Erwin Rahayu artmxarea@gmail.com",
  "license": "MIT",
  "bugs": {
    "url": "https://github.com/artmxra7/TestArkademy-3/issues"
  },
  "homepage": "https://github.com/artmxra7/TestArkademy-3#readme"
}
```

## Soal Nomor 6
Directory Soal 6 :
* [SQLITE](https://github.com/artmxra7/TestArkademy-3/tree/master/soal-6) - beserta documentasi dan query;

### Querry
```
sqlite3 (database_name);

CREATE TABLE users (
                id INTEGER,
                username STRING,
                CONSTRAINT users_PK PRIMARY KEY (id)
);

CREATE TABLE posts (
                id INTEGER,
                title STRING,
                content STRING,
                createdBy INTEGER,
                CONSTRAINT posts_PK PRIMARY KEY (id),
                CONSTRAINT posts_users_FK FOREIGN KEY (createdBy) REFERENCES users(id)
);

CREATE TABLE comments (
                id INTEGER,
                comment STRING,
                postId INTEGER,
                CONSTRAINT comments_PK PRIMARY KEY (id),
                CONSTRAINT comments_posts_FK FOREIGN KEY (postId) REFERENCES posts(id)
);

INSERT INTO users (username) VALUES ("Hesa Suryana");
INSERT INTO posts (title, content, createdBy) VALUES ("Wanita Di Serang Kadal", "wanita itu diserang kadal saat mengunjungi kebun binatang", 1); 
INSERT INTO comments (comment, postId) VALUES ("ah masa", 1);
INSERT INTO comments (comment, postId) VALUES ("serius?", 1);
INSERT INTO comments (comment, postId) VALUES ("bonbin mana?", 1);
INSERT INTO users (username) VALUES ("Erwin Rahayu");
```
## Soal Nomor 7

Request data dari data.db yang dibuat pada soal nomor 6 :
* [Arkademy Test](https://github.com/artmxra7/TestArkademy-3/tree/master/soal-7) - website akan berjalan di port: 8000;

### Installasi
* [Install node js](https://nodejs.org/en/download/) - Untuk Local Server
* Install required library
    ```
    npm init
    npm install express;
    ```
* Jalankan server dengan
    ```
    node index.js
    ```
### Built With
* [Kripken sql.js](https://github.com/kripken/sql.js/blob/master/js/sql.js) - SQLite compiled to JavaScript through Emscripten 
* [express](https://expressjs.com/) - Node.js web application framework

## Authors

* **ERWIN RAHAYU** - Dibuat untuk seleksi Arkademy #3



