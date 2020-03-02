Create container
```bash
cd docker/ && docker-compose up -d
```
Get into container
```bash
docker exec -it ruby-rails bash
```
Create new project
```bash
rails new blog
```
Navigate into project
```bash
cd blog/
```
Install dependencies
```bash
bundle install
```
Run rails server (Puma)
```bash
rails server -b 0.0.0.0