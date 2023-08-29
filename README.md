# Cisco AMP installation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-amp
  name: ansible-role-amp
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-amp

- Import role and override role variables, e.g.
```
- name: Setup amp
  roles:
    - role: ansible-role-amp
```

- All available role vars can be found in `defaults`
