# Boilerplatinator
Boilerplate for building website using customized Bootstrap Media Queries and Grid system with SASS.

## Notes for new Installation:
1. Download and Install [Git](https://git-scm.com/downloads)
2. Download and Install [Node.js](https://nodejs.org/en/)
( _Choose: Recommended for Most Users_ )

3. Create a file where you want to start your main project. 
4. Then **'Right Click'** on any white/empty space inside this file then choose **'Git Bash Here'**.  
5. A console will pop-up, then run this code to download the **'Boilerplatinator'** then close the console after downloading
	```console
	$git clone https://github.com/saysonjerald/boilerplatinator.git
	```
6. **Edit value** of this property 'name', 'version' and 'description' inside the package.json file
7. Rename the **'Boilerplatinator'** folder into your **project name**.
8. Open the **'Project Folder'** folder then **'Right Click'** on any white/empty space inside this file then choose **'Git Bash Here'**. 
	```javascript
	$npm install live-server -g
	```
9. Install Node Modules for this boilerplate.
  	```javascript
	$npm install 
	```
10. Delete the _.git_ folder, sometimes it's hidden.

## Notes for Development
1. To activate **LiveServer** type:
	```javascript
	$npm run devserver
	```
2. To activate **SASS Compiler** :
	```javascript
	$npm run watch:sass
	```
3. I recommend to activate  **BOTH** in one single CLI ( _parallel mode_ ) :
 	```javascript
	$npm run start
	```
4. Uncomment **'No Internet Script'** in index.html if you have no internet connection

5. **Use CDN** as much as you can or else I will kill YOU!

6. Use **BEM Architecture** | Please make your life easier

## Notes for Production
1.  **Compile** your SASS to CSS
	```javascript
	$npm run compile:sass
	```
	_output: sass/main.css_

2.  **Merge** all your CSS into one CSS file to reduce HTTP Requests - this will make your website load faster
	```javascript
	$npm run concat:css
	```
	_output: css/style.concat.css_

3.  This will make your website a higher chance to **run on unsupported browsers**.
	```javascript
	$npm run prefix:css
	```
	_output: css/style.prefix.css_

4.  **Compressing** the CSS File will make CSS execute faster on browsers
	```javascript
	$npm run compress:css
	```
	_output: css/style.css_

5.  **Run all Scripts** above using this command - _I recommend to run this command for production purposes_
	```javascript
	$npm run build:css
	```
	_output: css/style.css_

## Media Queries
* Grid breakpoints
```CSS
xxxs: 0,
xxs: 320px,
xs: 568px,
sm: 667px,
md: 768px,
lg: 992px,
xl: 1200px,
xxl: 1440px,
xxxl: 1600px
```

* Container Max-Width
```CSS
xxxs: 319px,
xxs: 414px,
xs: 568px,
sm: 608px,
md: 738px,
lg: 868px,
xl: 1092px,
xxl: 1330px,
xxxl: 1540px
```

Note: Don't be afraid to modify or add containers and breakpoint. 

* Media Query
```SCSS
//max-width
@include respond-below($breakpoint-value){
    property: value;
}

//min-width
@include respond-above($breakpoint-value){
    property: value;
}

//between min and max width
@include respond-between($lower, $upper){
    property: value;
}
```

### END