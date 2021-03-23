# pushgateway

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/pushgateway/status.svg)](https://drone.osshelp.ru/ansible/pushgateway)

Role for pushgateway_exporer installation.

## Usage (example)

```yaml
    - role: pushgateway
```

## Available parameters

### Main

| Param | Default | Description |
| -------- | -------- | -------- |
| `pushgateway_exporter_setup` | `full` | Setup mode. See [OSSHelp KB article](https://oss.help/kb4895) |
| `pushgateway_params.listen_address` | `0.0.0.0:9091` | Port to listen on. |
| `pushgateway_params.log_level` | `info` | Log level. |
| `pushgateway_params.log_format` | `logfmt` | Log format. |

### Persistence control

| Param | Default | Description |
| -------- | -------- | -------- |
| `pushgateway_persistence.enabled` | `true` | Whether to enable saving metrics to file (to avoid loosing them on restarts). |
| `pushgateway_persistence.interval` | `5m` | Interval of saving metrics to file. |
| `pushgateway_persistence.dir` | `/var/lib/pushgateway` | Directory, that will be created for metric files storage. |
| `pushgateway_persistence.file` | `persistent.metrics` | File name to dump metrics to. |

## FAQ

...

## Useful links

- [Official documentation](https://github.com/prometheus/pushgateway)
- [Our article](https://oss.help/kb6756)

## TODO

...

## License

GPL3

## Author

OSSHelp Team, see <https://oss.help>
