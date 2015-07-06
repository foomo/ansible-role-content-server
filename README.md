# Ansible Content server Role

[![Build Status](https://travis-ci.org/foomo/ansible-role-content-server.png?branch=master)](https://travis-ci.org/foomo/ansible-role-content-server)

> `content-server` is an [ansible](http://www.ansible.com) role which:
>
> * installs content-server

## Installation

Using `ansible-galaxy`:

```
$ ansible-galaxy install foomo.content-server
```

Using `requirements.yml`:

```
- src: foomo.content-server
```

Using `git`:

```
$ git clone https://github.com/foomo/ansible-content-server.git foomo.content-server
```

## Dependencies

* Ansible >= 1.9

## Variables

Here is a list of all the default variables for this role, which are also available in `defaults/main.yml`.

```
# package name (version)
content_server_package: content-server
```

## Handlers

These are the handlers that are defined in `handlers/main.yml`.

* `restart content-server`

## Example playbook

```
- hosts: all
  sudo: yes
  roles:
    - foomo.content-server
```

## Testing

```
$ git clone https://github.com/foomo/ansible-role-content-serverserver.git
$ cd ansible-content-server
$ vagrant up
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests and examples for any new or changed functionality.

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## License
Copyright (c) foomo under the LGPL 3.0 license.
