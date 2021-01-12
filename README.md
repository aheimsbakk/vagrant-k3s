# vagrant-k3s

Simple setup to start single k3s node in Vagrant with Ansible.

## Usage

```bash
vagrant up
```

## Advanced

If you have both `apt-cache-ng` and `docker.io/registry` running as caching proxies on a machine; using for example https://github.com/aheimsbakk/vagrant-apt-cacher-ng.

```bash
PROXY=proxy.local vagrant up
```

### Expected ports

`proxy.local` uses these ports.

| service | port |
| --- | ---|
| `apt-cacher-ng` | 3142 |
| `docker.io/registry` | 5000 |
