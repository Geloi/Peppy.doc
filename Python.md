Python comes with Raspbian distribution therefore there is no need to install it separately. The Peppy player was written using Python syntax from version 3. But the default Python version is 2.7. So if you just start Python from command line the version 2.7 will be in use. There is the symbolic link which points to version 2.7 - /usr/bin/python. That link should point to version 3 instead. To do that run the following command:
```
sudo ln -s -f /usr/bin/python3.4 /usr/bin/python
```
