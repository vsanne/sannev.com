### Environment Variables

WordPress environment variables. See the [official image](https://hub.docker.com/_/wordpress/) for additional information.

- `WORDPRESS_DB_NAME`: Name of database used for WordPress in MariaDB
- `WORDPRESS_TABLE_PREFIX`: Prefix appended to all WordPress related tables in the `WORDPRESS_DB_NAME` database
- `WORDPRESS_DB_HOST `: Hostname of the database server / container
- `WORDPRESS_DB_PASSWORD `: Database password for the `WORDPRESS_DB_USER`. By default 'root' is the `WORDPRESS_DB_USER`.

```yaml
    environment:
      - WORDPRESS_DB_NAME=${WORDPRESS_DB_NAME}
      - WORDPRESS_TABLE_PREFIX=${WORDPRESS_TABLE_PREFIX}
      - WORDPRESS_DB_HOST=${WORDPRESS_DB_HOST}
      - WORDPRESS_DB_USER=${WORDPRESS_DB_USER}
      - WORDPRESS_DB_PASSWORD=${WORDPRESS_DB_PASSWORD}
```

## <a name="site"></a>Running site

```
docker-compose up
```

### Initial WordPress setup

Navigate your browser to [http://127.0.0.1](http://127.0.0.1) and follow the installation prompts

1. Set language

    <img width="80%" alt="Select language" src="https://user-images.githubusercontent.com/5332509/44045885-f47a89fe-9ef7-11e8-8dae-0df0bfb269de.png">
2. Create an administrative user

    <img width="80%" alt="Create admin user" src="https://user-images.githubusercontent.com/5332509/44045887-f4897cfc-9ef7-11e8-89c6-cfc96cfc9ca0.png">

3. Success

    <img width="80%" alt="Success" src="https://user-images.githubusercontent.com/5332509/44045888-f49b344c-9ef7-11e8-9d65-39517f521d85.png">
    
4. Log in as the administrative user, dashboard, view site

    <img width="80%" alt="First login" src="https://user-images.githubusercontent.com/5332509/44045889-f4a71992-9ef7-11e8-8f5d-8ab16da481c2.png">
    
    <img width="80%" alt="Site dashboard" src="https://user-images.githubusercontent.com/5332509/44045890-f4b4b264-9ef7-11e8-935b-cbc546cd9e00.png">
    
    <img width="80%" alt="View site" src="https://user-images.githubusercontent.com/5332509/44045891-f4c5f90c-9ef7-11e8-88e4-fc8cfb61ea7d.png">
    
    
Once your site is running you can begin to create and publish any content you'd like in your WordPress instance.