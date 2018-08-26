# ELK 6.3

- `x-pack` support ouf of the box (Security and Monitoring)

## Installation & setup
Run `docker-compose up -d`.

### Generate passwords
1. Run the `docker exec -it elasticsearch bin/elasticsearch-setup-passwords auto` to generate the login credentials.
3. (temporary) Update elasticsearch credentials at `kibana/config.yml`
   - `elasticsearch.username` and `elasticsearch.password`

### Security
By default you have 4 users created: `elastic`, `kibana`, `beats_system`, `logstash_system`.

Feel free to manage these users and their roles in the `Management -> Users` or `Management -> Roles` section.
