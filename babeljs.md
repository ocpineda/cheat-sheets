#install babel
npm install -g babel-cli


npm install --save-dev babel-plugin-transform-flow-strip-types

echo '{"plugins": ["transform-flow-strip-types"]}' > .babelrc

#run transpiler in the background
babel --watch=./src --out-dir=./build
