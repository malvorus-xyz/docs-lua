# fs

## Reference

| Call | Description | Source |
| --- | --- | --- |
| `fs.append(...)` | fs.append(path, data): bool | [FsAppend](base/scripts/api/fs.cpp#L176) |
| `fs.create_dir(...)` | fs.create_dir(path): bool | [FsCreateDir](base/scripts/api/fs.cpp#L268) |
| `fs.exists(...)` | fs.exists(path): bool | [FsExists](base/scripts/api/fs.cpp#L224) |
| `fs.get_files(...)` | fs.get_files(path = ""): table | [FsGetFiles](base/scripts/api/fs.cpp#L288) |
| `fs.is_dir(...)` | fs.is_dir(path): bool | [FsIsDir](base/scripts/api/fs.cpp#L253) |
| `fs.is_file(...)` | fs.is_file(path): bool | [FsIsFile](base/scripts/api/fs.cpp#L238) |
| `fs.read(...)` | every path is resolved inside "<scripts>/data/", traversal is rejected fs.read(path): string \| nil | [FsRead](base/scripts/api/fs.cpp#L96) |
| `fs.remove(...)` | fs.remove(path): bool | [FsRemove](base/scripts/api/fs.cpp#L210) |
| `fs.write(...)` | fs.write(path, data): bool | [FsWrite](base/scripts/api/fs.cpp#L144) |
