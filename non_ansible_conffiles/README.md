This folder contains the config files that are not (yet) automatically deployed through ansible.

*sika_api.service* is the gunicorn service file. Should be placed to /etc/systemd/system/sika_api.service

The service can be started with
```
sudo systemctl enable sika_api
sudo systemctl start sika_api
```

*heitto* is the nginx conf file. Should be placed to /etc/nginx/sites-available/heitto

The site can be enabled with
```
sudo ln -s /etc/nginx/sites-available/heitto /etc/nginx/sites-enabled/
sudo nginx -t # Tests the config files
sudo systemctl restart nginx
```

