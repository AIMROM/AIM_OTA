# AIMROM OTA repository

Official maintainers can do a Pull Request here containing device JSON and changelog file to enable OTA support.

Sample format of `<device>.json`:

```
{
  "response": [
    {
      "datetime": 0000000000, // values as given on ro.build.date.utc
      "filename": "AIM-System-V4.0-Official-<device>-20200403-1800.zip",
      "id": "123456789abcdef0123456789abdcdef", // MD5 of your build
      "size": 123456789, // size in bytes
      "url": "https://sourceforge.net/projects/aim-rom-ten/files/<device>/AIM-System-V4.0-Official-<device>-20200403-1800.zip/download",
      "version": "V4.0"
    }
  ]
}
```
