# Office2016 16.11 for macOS VL2 license

2018-04-25

## ref

- VLSC ref: https://blog.csdn.net/cneducation/article/details/50573649
- License ref: https://bbs.feng.com/read-htm-tid-10731033.html

## activate

1. install Office2016 for mac with Office Suite Install, but **DO NOT RUN OFFICE AFTER INSTALLED**
   - manual download ref: https://macadmins.software/

```bash
brew cask install microsoft-office
```

2. copy license file `com.microsoft.office.licensingV2.plist` to `Preferences`

```bash
# md5(com.microsoft.office.licensingV2.plist) = a8f1283303838b4d3bd943775e463239
cp com.microsoft.office.licensingV2.plist /Library/Preferences/

# or download it in library by command line
curl -sSL git.io/office16-plist -o /Library/Preferences/com.microsoft.office.licensingV2.plist
```

3. run the office app
