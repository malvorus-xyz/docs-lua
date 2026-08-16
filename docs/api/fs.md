# fs

## Reference

| Call | Description |
| --- | --- |
| `fs.append(...)` | fs.append(path, data): bool |
| `fs.create_dir(...)` | fs.create_dir(path): bool |
| `fs.exists(...)` | fs.exists(path): bool |
| `fs.get_files(...)` | fs.get_files(path = ""): table |
| `fs.is_dir(...)` | fs.is_dir(path): bool |
| `fs.is_file(...)` | fs.is_file(path): bool |
| `fs.read(...)` | every path is resolved inside "&lt;scripts&gt;/data/", traversal is rejected fs.read(path): string \| nil |
| `fs.remove(...)` | fs.remove(path): bool |
| `fs.write(...)` | fs.write(path, data): bool |
