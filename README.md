# clamav

This role installs and configures a clamav daemon including freshclamd for database updates

## Requirements

Arch Linux or Ubuntu

## Role Variables

| Name            | Default/Required      | Description                          |
|-----------------|:---------------------:|--------------------------------------|
| `clamav_checks` | `12`                  | Database updates per day             |
| `clamav_mirror` | `database.clamav.net` | Database mirror to use for freshclam |

## Example Playbook

```yml
- hosts: av
  roles:
  - clamav
     clamav_checks: 24
```

## License

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

## Author Information

- [Janne Heß](https://github.com/dasJ)
