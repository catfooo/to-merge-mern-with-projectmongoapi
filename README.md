# .....

# current problem with this repo
i was able to run the server, without crashing app.
but it has two error (timeout, whitelist) in a row, 
so cant rly assure this is working or not
following is what i got from the terminal





 project-mongo-api git:(main) npm run dev

> project-mongo-api@1.0.0 dev
> nodemon server.js --exec babel-node

[nodemon] 3.0.2
[nodemon] to restart at any time, enter `rs`
[nodemon] watching path(s): *.*
[nodemon] watching extensions: js,mjs,cjs,json
[nodemon] starting `babel-node server.js`
Before connecting to MongoDB
Connecting to MongoDB using URL: mongodb+srv://deletedidforupload:deletedpwforuploadingpurpose@cluster0.0olueje.mongodb.net/happyThoughts?retryWrites=true&w=majority
After connecting to MongoDB
Starting database seeding...
(node:83055) [DEP0040] DeprecationWarning: The `punycode` module is deprecated. Please use a userland alternative instead.
(Use `node --trace-deprecation ...` to show where the warning was created)
(node:83055) [MONGOOSE] DeprecationWarning: Mongoose: the `strictQuery` option will be switched back to `false` by default in Mongoose 7. Use `mongoose.set('strictQuery', false);` if you want to prepare for this change. Or use `mongoose.set('strictQuery', true);` to suppress this warning.
Server running on http://localhost:8080
Error seeding database: MongooseError: Operation `books.deleteMany()` buffering timed out after 10000ms
    at Timeout.<anonymous> (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/mongoose/lib/drivers/node-mongodb-native/collection.js:175:23)
    at listOnTimeout (node:internal/timers:573:17)
    at processTimers (node:internal/timers:514:7)
MongoDB connection error: MongooseServerSelectionError: Could not connect to any servers in your MongoDB Atlas cluster. One common reason is that you're trying to access the database from an IP that isn't whitelisted. Make sure your current IP address is on your Atlas cluster's IP whitelist: https://www.mongodb.com/docs/atlas/security-whitelist/
    at NativeConnection.Connection.openUri (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/mongoose/lib/connection.js:825:32)
    at /Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/mongoose/lib/index.js:414:10
    at /Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/mongoose/lib/helpers/promiseOrCallback.js:41:5
    at new Promise (<anonymous>)
    at promiseOrCallback (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/mongoose/lib/helpers/promiseOrCallback.js:40:10)
    at Mongoose._promiseOrCallback (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/mongoose/lib/index.js:1290:10)
    at Mongoose.connect (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/mongoose/lib/index.js:413:20)
    at Object.<anonymous> (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/server.js:18:10)
    at Module._compile (node:internal/modules/cjs/loader:1376:14)
    at Module._compile (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/pirates/lib/index.js:117:24)
    at Module._extensions..js (node:internal/modules/cjs/loader:1435:10)
    at Object.newLoader [as .js] (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/pirates/lib/index.js:121:7)
    at Module.load (node:internal/modules/cjs/loader:1207:32)
    at Function.Module._load (node:internal/modules/cjs/loader:1023:12)
    at Function.runMain (node:internal/modules/run_main:135:12)
    at Object.<anonymous> (/Users/catfood/project-mongo-api-connectiontest2/project-mongo-api/node_modules/@babel/node/src/_babel-node.ts:222:12)
    at Module._compile (node:internal/modules/cjs/loader:1376:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1435:10)
    at Module.load (node:internal/modules/cjs/loader:1207:32)
    at Function.Module._load (node:internal/modules/cjs/loader:1023:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:135:12)
    at node:internal/main/run_main_module:28:49 {
  reason: TopologyDescription {
    type: 'ReplicaSetNoPrimary',
    servers: Map(3) {
      'ac-pduuxjk-shard-00-00.0olueje.mongodb.net:27017' => [ServerDescription],
      'ac-pduuxjk-shard-00-01.0olueje.mongodb.net:27017' => [ServerDescription],
      'ac-pduuxjk-shard-00-02.0olueje.mongodb.net:27017' => [ServerDescription]
    },
    stale: false,
    compatible: true,
    heartbeatFrequencyMS: 10000,
    localThresholdMS: 15,
    setName: 'atlas-hjl0mu-shard-0',
    maxElectionId: null,
    maxSetVersion: null,
    commonWireVersion: 0,
    logicalSessionTimeoutMinutes: null
  },
  code: undefined
}




# Project Mongo API..........

Replace this readme with your own information about your project.

Start by briefly describing the assignment in a sentence or two. Keep it short and to the point.

## The problem

Describe how you approached to problem, and what tools and techniques you used to solve it. How did you plan? What technologies did you use? If you had more time, what would be next?

## View it live

Every project should be deployed somewhere. Be sure to include the link to the deployed project so that the viewer can click around and see what it's all about.
