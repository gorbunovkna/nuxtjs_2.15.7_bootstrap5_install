# nuxtjs_2.15.7_bootstrap5_install
//install nuxt
npm init nuxt-app myapp

create folder 
/myapp/assets/css/main.scss

insert in file main.scss 
@import '~bootstrap/scss/bootstrap';
//save file

create folder
/myapp/static/js/
copy js files from 
cp myapp/node_modules/bootstrap/dist/js/* /myapp/static/js/

edit 
./myapp/package.json
{
  "name": "myapp",
  "version": "1.0.0",
  "private": true,
  "scripts": {
    "dev": "nuxt",
    "build": "nuxt build",
    "start": "nuxt start",
    "generate": "nuxt generate"
  },
  "dependencies": {
    "@nuxtjs/axios": "^5.13.6",
    "@nuxtjs/pwa": "^3.3.5",
    "@nuxtjs/sitemap": "^2.4.0",
    "bootstrap": "^5.0.0-beta3",
    "bootstrap-next": "^1.0.5",
    "core-js": "^3.15.1",
    "nuxt": "^2.15.7"
  },
  "devDependencies": {
    "fibers": "^5.0.0",
    "sass": "1.32.13",
    "sass-loader": "^10.2.0",
    "webpack": "^4.46.0"
  }
}

npm install 
edit nuxt.config.js add bootstrap 5
head: {
    script: [
      {
        src: '/js/bootstrap.js', type: "text/javascript"
      }
    ]

  },
add 
 css: [
    '@/assets/css/main',
  ],
  
  profit!
  
