# Dubzland: Ruby
[![Gitlab pipeline status (self-hosted)](https://git.dubzland.net/dubzland/ansible-role-ruby/badges/master/pipeline.svg)](https://git.dubzland.net/dubzland/ansible-role-ruby)

Installs and configures Ruby from source.

## Requirements

Ansible 2.2 or higher.

## Role Variables

Available variables are listed below, along with their default values (see
    `defaults/main.yml` for more info):

### dubzland_ruby_version

```yaml
dubzland_ruby_version: "2.6.3"
```

Specific version of Ruby to install.

### dubzland_ruby_source_root

```yaml
dubzland_ruby_source_root: "/usr/local/src"
```

Directory used to store tarballs, as well as extract and build source tree.

### dubzland_ruby_minor_version

```yaml
dubzland_ruby_source_url: "https://cache.ruby-lang.org/pub/ruby/2.6/ruby-2.6.3.tar.gz"
```

URL used to download Ruby source tarball.

### dubzland_ruby_source_sha256sum

```yaml
dubzland_ruby_source_sha256sum: "577fd3795f22b8d91c1d4e6733637b0394d4082db659fccf224c774a2b1c82fb"
```

SHA256 checksum used to validate the downloaded source tarball.

### dubzland_ruby_bundler_version

```yaml
dubzland_ruby_bundler_version: "1.17.3"
```

Version of Bundler to install.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: dubzland.ruby
```

## License

MIT

## Author

* [Josh Williams](https://codingprime.com)
