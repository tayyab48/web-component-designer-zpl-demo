## Developing

  * Install dependencies
```
  $ npm install
```
  * Run the app in a local server
``` 
 $ npm run start
```

* Build the Project: Compile the TypeScript files and prepare the build directory.

```
npx tsc
```
* Copy Necessary Files: Copy the required files to the build directory.
```
npx copyfiles --verbose "node_modules/**/*.js" build/default
npx copyfiles --verbose "node_modules/**/*.json" build/default
npx copyfiles --verbose "dist/**/*.js" build/default
npx copyfiles --verbose "dist/**/*.json" build/default
npx copyfiles --verbose "*.html" build/default
npx copyfiles --verbose "node_modules/**/*.css" build/default
npx copyfiles --verbose "node_modules/**/*.png" build/default
npx copyfiles --verbose "node_modules/**/*.svg" build/default
npx copyfiles --verbose "node_modules/**/*.gif" build/default
npx copyfiles --verbose "node_modules/**/*.jpg" build/default
npx copyfiles --verbose "node_modules/**/*.woff" build/default
npx copyfiles --verbose "node_modules/**/*.ttf" build/default
npx copyfiles --verbose "assets/**/*.png" build/default
npx copyfiles --verbose "assets/**/*.svg" build/default
npx copyfiles --verbose "assets/**/*.css" build/default
npx copyfiles --verbose "*.json" build/default

```

* Upload to S3
# Upload build/default to s3