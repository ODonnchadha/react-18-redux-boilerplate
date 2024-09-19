# React-18-Redux-Boilerplate

1. To run and test the app on your local machine (http://localhost:8080):
    ```javascript
    npm run start
    ```
    This will start a server instance and begin listening for connections from localhost on port `8080`.
2. To build/deploye the app, you can run:
    ```javascript
    npm run build
    ```
    This will place all files needed for deployment into the `/dist` directory.

## Project Structure
```sh
├── public  
    ├── favicon.ico
    ├── index.html              # html template for the app
    ├── thumbnail.jpg           # an image will be used in og:image meta tag
├── src                         # Source code.
    ├── components              # React components
    ├── contexts                # React contexts
    ├── store                   # Redux store
        ├── ToDo                # contains reducer, selectors and thunks for ToDo "slice" of the redux store
        ├── configureStore.ts   # configure the app's redux store
        ├── getPreloadedState.ts 
        ├── rootReducers.ts     # combine reducers from all slices
    ├── styles                  # app-wide styles
    ├── types                   # type definitions
    └── index.tsx               # entry point for the app
├── .babelrc                    # Babel configuration
├── .eslintrc.js                # ESLint configuration
├── .prettierrc.js              # Prettier configuration
├── tsconfig.json               # TypeScript configuration
├── webpack.config.js           # Webpack configurations
├── tailwind.config.js          # Tailwind CSS configurations
├── postcss.config.js           # PostCSS configurations
```