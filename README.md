# YAWAF - Yet Another Web Application Framework

Minimalist Middileware Framework

![z](https://img.icons8.com/fluent/96/000000/server.png)

## Why?
Why not?

# Installation
```sh
> npm i yawaf
```
# Usage

```TS
import App from 'yawaf'
// or const { App } = require('yawaf')
// or const App = require('yawaf').default
// or const App = require('yawaf').App

// Initialize App
const app = new App()

// Add yout middleware
app.use((req, res, next) => {
    // Do stuff like logging and auth here
    next()
})

app.use('/', (req, res) => {
    // Write code
    res.end('This is a cool response')
})

app.use('/hi', (req, res) => {
    res.end('Hi. Cool endpoint, right?')
})


// Make the app bind to a PORT
app.listen(process.env.PORT || 5000)

//Pofit!
```

## Better Docs comming soon  -PRs Welcome!