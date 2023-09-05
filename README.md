  # Python GetContact API

### Require
- Rooted Emulator (Im using LDPlayer)
- ADB

### How To Get Token and AES Key
- adb shell
- cat /data/data/app.source.getcontact/shared_prefs/GetContactSettingsPref.xml
- FINAL_KEY = AES Key | Token = Token
- Change your AES Key and Token in getcontact/config.py and dump/tokens.yaml (tokens and keys will rolling to another user if remain count runs out.)

### How To Use
- ```pip install -r requirements.txt```
- ```python3 main.py -p +628xxxxxxxxx -j```

### Output
- ```{'name': None, 'phoneNumber': '+628xxxxxxxxx', 'country': 'ID', 'displayName': 'GTC Display Name', 'profileImage': 'https://s3-v2.cdngtc.com/profile_img_v2_61444632133f6ee34601d9e229ff79d1e67ae2b77.64f01b38b3e52.png', 'email': None, 'is_spam': False, 'tags': ['Tag 1', 'Tag 2']}```
