Instructions to Clone this repo
=======

The following are step-by-step instructions to make a clone of this repo and push it to the NPM registry

### Pre-requisites:

	1. A github.com account
	2. An npmjs.com account
	3. NodeJs & NPM (installed on your computer)
	4. Git (installed on your computer)


### 1. Click the fork button on this repo https://github.com/ziwer1/yuglify

### 2. Clone from the fork you created above in step 1 using git.

### 3. Open `package.json` file in your editor and edit the following:
```
"name": "@ziwer1/yuglify"  --change using the format: @<npm account user or organisation name or scope>/<package name> e.g. @user4/yuglify
"description": "A fork of yuglify by YUI",
...
"bugs": {
	"url": "https://github.com/ziwer1/yuglify/issues"  --change ziwer1/yuglify to match the github fork you just made.
}
...
"repository": {
	....
	"url": "git+https://github.com/ziwer1/yuglify.git" --change ziwer1/yuglify to match the github fork you just made.
},
"homepage": "https://github.com/ziwer1/yuglify#readme", --change ziwer1/yuglify to match the github fork you just made.
...
"author": "ziwer1", --change ziwer1 to your name.
```

### 4. Commit these changes using git

### 5. Make any other changes to the package and commit them.

Update the package version no. in `package.json` with every change.

*If you don't update the version no. you will not be able to push to the npm registry.*

Edit the version no. by opening `package.json` in your editor.

### OR

Run the following command AFTER committing a change to update the package version no. in package.json.

`npm version patch -m 'update package version'`
	
*This command will update the version no. in package.json and make a commit.*


### 6. Login on the npm cli
		
`npm login`

### 7. Publish to the npm registry

`npm publish`
	
### OR
	
If you want your package to be available publicly:

`npm publish --access public` 





REFERENCES:
-----------
You can read about npm scopes [here](https://docs.npmjs.com/about-scopes)

