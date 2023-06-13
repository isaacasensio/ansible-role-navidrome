Navidrome
=========

Navidrome is an open source web-based music collection server and streamer. It gives you freedom to listen to your music collection from any browser or mobile device. It's like your personal Spotify!

This Ansible role installs Navidrome as a Docker service.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
navidrome_image: "lscr.io/linuxserver/navidrome:latest"
```
The version of the docker image to run as a container.

```
navidrome_host_config_path: /etc/navidrome
```
Host path which stores navidrome configuration.

```
navidrome_host_data_path: /var/lib/navidrome
```
Host path which stores navidrome data.

```
navidrome_container_user: navidrome
```
user running the container 

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - iasensio.navidrome

License
-------

MIT

