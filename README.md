# nuxt1.4.4-firebase

## Description

The project works on the framework using __Nuxt.js__ to build a client-side.
You'll also see basic setting for __Cloud Functions for Firebase__.

## Install dependencies

You need install dependencies under ```client``` and ```functions``` directories. The first one is for __Nuxt.js__ project, and the second one is for __Cloud Functions for Firebase__.

```
cd client
npm i (or yarn install)
```

```
cd functions
npm i (or yarn install)
```

## Run Nuxt with the development mode

Run npm run dev for a dev server. In this project, the command contains ```DEV=1``` for changing the mode.

```
cd client
npm run dev
```

## Run functions locally

First of all, you need build Nuxt.js project and copy static files to public directory. For this, run the following command.

```
cd client
npm run build
```

In this project, the command contains both of build and copy. 

Then, you can run functions locally to test with the fallowing command.

```
(At client directory)
firebase serve --only hosting,functions
```

See [more information](https://firebase.google.com/docs/functions/local-emulator?hl=en).

## Author

okapie