# Commands Used in BES Serial Exercise Debugging

Here is a list of terminal commands used during debugging and development:

```bash
docker compose down --volumes
```

```bash
docker compose build --no-cache
```

```bash
docker compose up
```

```bash
docker compose run --rm simulated_dut
```

```bash
docker compose run --rm test_fixture
```

```bash
python3 main.py
```

```bash
git status
```

```bash
### creates a tree of main files great for showing a directory to AI and only shows main files

git ls-tree -r --name-only HEAD 

tree -L 2
```

```bash
ls -la .git
```

```bash
docker build -t simulated_dut .
```

```bash
docker run -it --rm simulated_dut
```

```bash
docker ps -a
```

```bash
docker logs <container_id>
```

```bash
docker exec -it <container_id> /bin/bash
```

