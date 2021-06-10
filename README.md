# Docker with:
- NGINX alpine
- PHP-7.4-FPM or high
- MySQL
- MySQL - auto backups
- Phpmyadmin

To run: `docker-compose up`

## Project structure
```
docker/
├─ mysql/
│    ├─ backups/ - here are automatic backups
│    ├─ config/ - my.ini config
│    ├─ data/ - the data of mysql service
│    ├─ resources/ - put here your database if you want import it via CLI
├─ nginx/
│    ├─ config/ - config files of web server
├─ php/
│    ├─ config/ - config files like php.ini
└─ web/ - it's main directory of your website
```