# Examples

## Syncthing - [github.com/syncthing/syncthing](https://github.com/syncthing/syncthing)

### Focusing package _upgrade_

![syncthing example output](images/syncthing_focus.png)

```
go-callvis -focus upgrade -limit github.com/syncthing/syncthing github.com/syncthing/syncthing/cmd/syncthing | dot -Tpng -o syncthing_focus.png
```

--------------------------------------------------------------------------------

### Grouping by _packages_

![syncthing example output pkg](images/syncthing_group.png)

```
go-callvis -focus upgrade -group pkg -limit github.com/syncthing/syncthing github.com/syncthing/syncthing/cmd/syncthing | dot -Tpng -o syncthing_group.png
```

--------------------------------------------------------------------------------

### Ignoring package _logger_

![syncthing example output ignore](images/syncthing_ignore.png)

```
go-callvis -focus upgrade -group pkg -ignore github.com/syncthing/syncthing/lib/logger -limit github.com/syncthing/syncthing github.com/syncthing/syncthing/cmd/syncthing | dot -Tpng -o syncthing_ignore.png
```
