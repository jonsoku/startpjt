# first
    1. php artisan preset react
    2. npm install && npm run dev
    3. npm install react-router-dom && npm install axios && npm install styled-components && npm install styled-reset && npm install react-js-pagination && npm install react-player

# .env
    DB_CONNECTION=mysql
    DB_HOST=laravel.cim78dtgz3dv.ap-northeast-1.rds.amazonaws.com
    DB_PORT=3306
    DB_DATABASE=blog
    DB_USERNAME=the2792
    DB_PASSWORD=canyou12

# AppServiceProvider.php
    <?php

    namespace App\Providers;

    use Illuminate\Support\Facades\Schema;
    use Illuminate\Support\ServiceProvider;

    class AppServiceProvider extends ServiceProvider
    {
        public function register()
        {
            //
        }

        public function boot()
        {
            Schema::defaultStringLength(191);
        }
    }

# welcome.blade.php
     <body>
            <div id="example"></div>
            <script src="{{ asset('js/app.js') }}" defer></script>
    </body>


# 필요한 extension
    

# babel
    .babelrc 생성

    {
    "presets": ["@babel/preset-env", "@babel/preset-react"],
    "plugins": ["@babel/plugin-proposal-class-properties"]
    }

# package.json
    "devDependencies": {
    "@babel/plugin-proposal-class-properties": "^7.4.0",
    "@babel/preset-env": "^7.4.2",
    "@babel/preset-react": "^7.0.0",
    "axios": "^0.18.0",
    "babel-plugin-transform-class-properties": "^6.24.1",
    "babel-preset-env": "^1.7.0",
    "babel-preset-react": "^6.24.1",
    "babel-preset-stage-1": "^6.24.1",
    "bootstrap": "^4.0.0",
    "cross-env": "^5.1",
    "jquery": "^3.2",
    "laravel-mix": "^4.0.7",
    "lodash": "^4.17.5",
    "popper.js": "^1.12",
    "prettier-eslint": "^8.8.2",
    "react": "^16.2.0",
    "react-dom": "^16.2.0",
    "resolve-url-loader": "^2.3.1",
    "sass": "^1.15.2",
    "sass-loader": "^7.1.0",
    "vue-template-compiler": "^2.6.10"
