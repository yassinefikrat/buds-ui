# buds-ui

> UI components for Knowledge Chef

## Build Setup

```bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run all tests
npm test
```

## Bit

```sh
bit init
bit login
bit add src/components/_ -t 'test/unit/specs/_'
bit status
bit import bit.envs/bundlers/vue --compiler
bit import bit.envs/testers/jest --tester
bit tag --all 1.0.0
bit export yassinefikrat.buds-ui
```



