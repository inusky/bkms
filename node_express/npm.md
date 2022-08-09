- [express](https://www.npmjs.com/package/express)

```javascript
const express = require('express');
const app = express();

app.get('/', function (req, res) {
  res.send('Hello World');
});

app.listen(3000);
```

-[nodemon](https://www.npmjs.com/package/nodemon)

`npm install --save-dev nodemon`

- [Mongoose](https://www.npmjs.com/package/mongoose)

`npm i mongoose@6.3.2` if requir a special version

```javascript
// Using Node.js `require()`
const mongoose = require('mongoose');

// Using ES6 imports
import mongoose from 'mongoose';
```

- [http](https://www.npmjs.com/package/http)
