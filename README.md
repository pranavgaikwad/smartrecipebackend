# Smart Recipe Recommender Backend

A mock backend for Smart Recipe Recommender

## Tech Spec

* Json Server
* Node.js 

### User APIs

Collection of users 

```json
{ 
    "users": [
        { 
            "_type": "user", 
            "id": "", 
            "name": "", 
            "email": "", 
            "password": "", 
            "salt": "", 
            "createdAt": "", 
            "updatedAt": "" 
        }
    ]
}
```

Sign Up API

```bash
POST /signup

Parameters : 
{
    "user": {
        "email": "",
        "password": "",
    }
}
```

Sign In API

```bash
POST /signin

Parameters : 
{
    "user": {
        "email": "",
        "password": "",
    }
}
```

### Ingredient APIs

Collection of ingredients

```json
{ 
    "ingredients": [
        { 
            "_type": "ingredient", 
            "id": "", 
            "name": "", 
            "qty": "", 
            "unit": "", 
            "createdAt": "", 
            "updatedAt": "" 
        }
    ]
}
```

Get list of ingredients

```bash
GET /ingredients

Headers: 
{
    X-Access-Token: "<ACCESS_TOKEN>",
}
```

Add new ingredient

```bash
POST /ingredients

Parameters : 
{
    "id": "<OPTIONAL>",
    "name": "",
    "qty": "",
    "unit": "",
}

Headers: 
{
    X-Access-Token: "<ACCESS_TOKEN>",
}
```

### Recipe API



## Installation & Usage

### Build Requirements

Make sure you have these packages installed in order to build the project

* npm
* yarn

#### Building the application

Make sure that the port 3001 is available. Run following commands to run the application

```bash
git clone 
cd smartrecipebackend
yarn start
```

#### Production Build

This application is only used in development.