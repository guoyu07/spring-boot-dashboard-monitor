## dashboard-monitor

Display the most relevant parts of your application infrastructure on one dashboard page.
UI part is inspired on dashing.
 
## Back-end Setup

With the help of the Spring boot developer tools, every class change will lead the embedded 
Tomcat to restart, so that an application hot-reload leads to quick developer turn around times 

     mvn --projects backend spring-boot:run
     

## Front-end Setup

For developing on the frontend side, it is very convenient to use the
webpack integrated hot-reload cycle, before packaging your app up for production:

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8000
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) 
and [docs for vue-loader](http://vuejs.github.io/vue-loader).
