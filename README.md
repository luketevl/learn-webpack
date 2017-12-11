# learn-webpack
Learn about webpack

# LINKS
- https://webpack.js.org/
- https://babeljs.io/


# UGLIFYJS
- **Minify** the script
- **Remove** unused imports

# WEBPACK DEV SERVER
- Create server
  - **--inline** | Live reload
  - **--open** | open automatic browser
```shell
webpack-dev-server --inline --open
```


# ENVIROMENTS
```javascript
const nodeENV = process.env.NODE_ENV || 'production';
new webpack.DefinePlugin({
          'process.env': { NODE_ENV: JSON.stringify(nodeENV) }
      })  
```

# SOURCEMAP
> Used to trace error in original file
```javascript
{devtool: 'source-map'}
```

# OBSERVATION
- Use env variables
  - ```NODE_ENV='development'``` npm run build
```javascript
process.env.NODE_ENV || 'production';
```

