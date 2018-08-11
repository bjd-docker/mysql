# MySQL image

## Usage

### docker-compose

```yaml
version: '3'

services:
  mysql:
    image: 'bjouhaud/mysql'
    hostname: 'mysql'
    ports:
      - '3306:3306'
    volumes:
      - 'mysql:/var/lib/mysql'
    environment:
      MYSQL_DATABASE: 'dev'
      MYSQL_USER: 'root'
      MYSQL_PASSWORD: ~
      MYSQL_ALLOW_EMPTY_PASSWORD: 1

volumes:
  mysql: ~
```
