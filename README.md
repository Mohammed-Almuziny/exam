## Error: Cannot find module '../db'

The solution

```
require("./db");
```

## Error: Cannot find module 'mongoose'

the solution : write in terminal

```
npm i mongoose
```

## Error: Cannot find module './../../db/models/todos'

the solution : in controller/todos line 1

```
const todoModel = require("./../../db/models/todo");
```

## Error: Cannot find module 'mongose'

the solution : in models/todo.js line 1

```
const mongoose = require("mongoose");
```

## TypeError: mongoose.module is not a function

the solution : in models/todo.js line 10

```
const todoModel = mongoose.model("Todo", todoSchema);
```

## Error: Route.get() requires a callback function but got a [object Undefined]

the solution : in controller/todos line 96

```
module.exports = {
```

## Error: Route.put() requires a callback function but got a [object Undefined]

the solution : in controller/todos line 103 and 104

```
  updateTodo,
};
```

## ReferenceError: morgan is not defined

the solution : in index.js after line 3

```
const morgan = require("morgan");
```

## Error: listen EACCES: permission denied 4000;

the solution : in .env

```
PORT=4000
```
