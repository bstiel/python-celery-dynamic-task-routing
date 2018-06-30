# Unit Testing Celery Tasks

This projects contains the source code examples accompanying the blog post: https://www.python-celery.com/2018/05/29/task-routing/.

Docker is highly recommended.

1. Bring up the docker stack:
```docker-compose up -d```

2. Execute example.py in one of the app-image containers:
```docker-compose exec worker-feeds python example.py --start_date=2018-01-01 --end_date=2018-05-29 --window=3```

3. Show logs:
```docker-compose logs```

4. Monitor tasks in flower:
[http://localhost:5555](http://localhost:5555)

If you run without docker, make sure you run the services
specified in the docker-compose.yml file individually and
adjust the environment variables, ports etc as required.