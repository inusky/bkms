- [ES6 Modules and How to Use Import and Export in JavaScript](https://www.digitalocean.com/community/tutorials/js-modules-es6)

> package.json settings

```json
  "type": "module",
```

> Examples

```js
import express from 'express';
import connectDB from './db/connectdb.js';
import web from './routes/web.js';
/*

const app = express();

const port = process.env.PORT || '8000';
const DATABASE_URL = process.env.DATABASE_URL || 'mongodb://localhost:27017';

connectDB(DATABASE_URL);
app.use(express.json());

app.use('/api', web);

app.listen(port, () => {
  console.log(`Server listening at http://localhost:${port}`);
});
*/
```

> Examples

>

```js
// module/packages
import mongoose from 'mongoose';
/*
const studentSchema = new mongoose.Schema({
  stuname: { type: String, required: true, trim: true },
  email: { type: String, required: true, trim: true },
});

const StudentModel = mongoose.model('student', studentSchema);

*/
export default StudentModel;
```

> Examples

```js
import StudentModel from '../models/Student.js';
/*
class StudentController {
  static getAllDoc = async (req, res) => {
    try {
      const result = await StudentModel.find();
      res.send(result);
    } catch (error) {
      console.log(error);
    }
  };
}
*/
export default StudentController;
```
