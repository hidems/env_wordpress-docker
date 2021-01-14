# How to start
```
docker-compose up -d
```

### Access: http://localhost:8080/

### phpmyadmin: http://localhost:8888/
Access with root and password

# Edit code
It is necessary to change authority.

Ex. Edit in directry `wp-content`
```
sudo chmod -R 777 wp-content
sudo chown {username}:{username} -R wp-content
```

# All in One WP Migration
Install `All in One WP Migration` in plugin menu.

### Change uploadable file size
Add this code in `.htaccess`

```
php_value upload_max_filesize 256M
php_value post_max_size 256M
php_value memory_limit 512M
php_value max_execution_time 300
php_value max_input_time 300
```