BROWSERIFY=./node_modules/.bin/browserify

run: install static/bundle.js
	node server.js

install: package.json
	npm i

static/bundle.js: debris.js
	$(BROWSERIFY) debris.js > static/bundle.js
	
