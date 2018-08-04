# cmsrs-laravel-vue
cms base on Laravel and Vue
	in progress ...

###Install:

1.
```bash
$git clone https://github.com/cmsrs/cmsrs-laravel-vue.git
```

2.
```bash
$cd cmsrs-laravel-vue && composer install
```

3.
```bash
$cp .env.example .env
```

in file .env chenge:


set 
APP_URL=http://cmsrs-laravel-vue.loc

set
DB_*

4.
```bash
$php artisan key:generate
```

5. 
add vhost (in apache):

```bash
        <VirtualHost *:80>
            ServerAdmin webmaster@localhost
            ServerName cmsrs-laravel-vue.loc
            #ServerAlias cmsrs-laravel-vue.loc
            DocumentRoot /var/www/cmsrs-laravel-vue/public
            <Directory /var/www/cmsrs-laravel-vue>
                Options Indexes FollowSymLinks MultiViews
                AllowOverride all
                Require all granted
            </Directory>
            ErrorLog /var/log/apache2/cmsrs-laravel-vue-error.log
            LogLevel error
            CustomLog /var/log/apache2/cmsrs-laravel-vue-access.log combined
        </VirtualHost>
```






Usefull scripts:

1.
change permission:
go.sh 

2.
show log:
go_log_err.sh 
