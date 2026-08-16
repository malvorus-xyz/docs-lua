# fs

## Reference

| Call | Description | Source |
| --- | --- | --- |
| `fs.append(...)` | fs.append(path, data): bool | [FsAppend](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L176) |
| `fs.create_dir(...)` | fs.create_dir(path): bool | [FsCreateDir](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L268) |
| `fs.exists(...)` | fs.exists(path): bool | [FsExists](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L224) |
| `fs.get_files(...)` | fs.get_files(path = ""): table | [FsGetFiles](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L288) |
| `fs.is_dir(...)` | fs.is_dir(path): bool | [FsIsDir](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L253) |
| `fs.is_file(...)` | fs.is_file(path): bool | [FsIsFile](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L238) |
| `fs.read(...)` | every path is resolved inside "&lt;scripts&gt;/data/", traversal is rejected fs.read(path): string \| nil | [FsRead](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L96) |
| `fs.remove(...)` | fs.remove(path): bool | [FsRemove](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L210) |
| `fs.write(...)` | fs.write(path, data): bool | [FsWrite](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/fs.cpp#L144) |
