# AIMROM OTA repository

Official maintainers can do a Pull Request here containing device JSON and changelog file to enable OTA support.

## Directory structure

```
AIM_OTA
|-- <device>
|   |-- changelog.txt (common for both)
|   |-- gapps.json (GApps variant)
|   `-- lucid.json (non-GApps variant)
```

## Sample JSON format

```
{
  "response": [
    {
      "datetime": 0000000000, // values as given on ro.build.date.utc
      "filename": "AIM-System-V4.1-Official-[Lucid|GApps]-<device>-20200425-0000.zip",
      "id": "123456789abcdef0123456789abdcdef", // MD5 of your build
      "size": 123456789, // size in bytes; ls -l your zip file and copy that
      "url": "https://sourceforge.net/projects/aim-rom-ten/files/<device>/AIM-System-V4.1-Official-[Lucid|GApps]-<device>-20200425-0000.zip/download",
      "version": "V4.1"
    }
  ]
}
```

**We deserve any rights to deny a Pull Request if it doesn't follow criteria shown here.**
