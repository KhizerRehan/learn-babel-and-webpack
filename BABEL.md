## Babel Updates:
- https://babeljs.io/docs/en/env/


```json
BOTH ARE SAME USE EITHER ONE OF OPTION:

=> .babelrc

{
    "presets": [
      "@babel/preset-env","@babel/preset-react"
    ]
}

=> webpack.config.js

{
   "test":"/\\.(js|jsx)$/",
   "exclude":"/node_modules/",
   "use":{
      "loader":"babel-loader",
      "options":{
         "presets":[
            "@babel/preset-env",
            "@babel/preset-react"
         ]
      }
   }
}
___