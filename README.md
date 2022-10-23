FR24
=========

Install Flightradar24 feeder  
Original repo for contributions at https://gitlab.com/drid/ansible-role-fr24.git, 

Role Variables
--------------
```yaml
fr24_key: Your FR24 key
fr24_sdr_ppm: PPM of sdr receiver
fr24_device_index: index of receiver if there are multiple
fr24_receiver: dvbt/sbs1tcp/sbs1usb/beast/beast-tcp/dvbt-mr
fr24_proc_args: any other arguments to pass
fr24_bs: yes/no
fr24_raw: yes/no
fr24_mlat: yes/no
fr24_mlat_without_gps: yes/no
fr24_logmode: Log level 0/1/2
```  
See [FR24 feeder manual](https://feed.flightradar24.com/fr24feed-manual.pdf) for details on these settings

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - { role: fr24, fr24_key: 768276342 }
```
License
-------

GPL-3.0
