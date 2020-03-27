# serving-HTML-page-404-error-page

https://www.udemy.com/course/nodejs-the-complete-guide/learn/lecture/11566312#questions
70 & 71

adding 'path' in app.js & routes folder's admin.js, shop.js
& add 404.html file in 'views' folder


in each js file, 
const path = require('path'); ///added
app.use((req, res, next) => {
    res.status(404).sendFile(path.join(__dirname, 'views', '404.html'));
}); ////revised with 'dirname'
