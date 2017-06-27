# add flow to project
npm install --save-dev flow-bin

# Run flow
npm run-script flow

# create flow project
flow init

# run ad-hoc checks on code and subfolders:

flow check

# ------ BABEL ------------------

#install babel
npm install -g babel-cli


npm install --save-dev babel-plugin-transform-flow-strip-types

echo '{"plugins": ["transform-flow-strip-types"]}' > .babelrc

#run transpiler in the background
babel --watch=./src --out-dir=./build
