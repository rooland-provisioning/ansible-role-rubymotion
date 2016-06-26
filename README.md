# rubymotion

Set [RubyMotion](http://www.rubymotion.com/) development up. Please note, that
this is unofficial role.

## Requirements

This role handles only RubyMotion necessary stuff, so things like installing
Ruby, RubyMine, etc. is out of the scope of this role.

## Role Variables

- rubymotion.platforms (required) -- list of platforms needed to be installed

## Example Playbook

```yaml
---
- hosts: localhost
  roles:
    - role: rooland-provisioning.rubymotion
      tags:
        - android
        - ios
        - osx
        - ruby
        - rubymotion
  vars:
    rubymotion:
      platforms:
        - platform_name:  apple
        - platform_name:  android
```

## License

BSD

## Author Information

### Mailo Svetel

- Usually idling on Freenode as lipoqil
- http://him.rlnd.cz
