# Learn Up - DevOps - homework 17

I wrote playbook1.yaml, plyabook2.yaml, playbook3.yaml for practice

other files belong to homework 17 (based on homework 15)

added https://galaxy.ansible.com/singleplatform-eng/users



## ansible-users
## Role to manage users on a system.

## Role configuration
- users_create_per_user_group (default: true) - when creating users, also
create a group with the same username and make that the user's primary
group.
- users_group (default: users) - if users_create_per_user_group is not set,
then this is the primary group for all created users.
- users_default_shell (default: /bin/bash) - the default shell if none is
specified for the user.
- users_create_homedirs (default: true) - create home directories for new
users. Set this to false if you manage home directories separately.
- authorized_keys_file (default: .ssh/authorized_keys) - Set this if the
ssh server is configured to use a non standard authorized keys file.