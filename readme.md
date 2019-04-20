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
