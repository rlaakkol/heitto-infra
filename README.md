# heitto-infra

## Usage

To setup a fresh host, complete the following steps:

1. Create a file called `ansible.cfg` with the following contents
  ```
  [defaults]
  remote_user = <your username on the host>
  hostfile = hosts
  ```
2. Run the users playbook
  ```sh
  $ ansible-playbook users.yml -v
  ```
3. Run the server playbook
  ```sh
  $ ansible-playbook server.yml -v
  ```
