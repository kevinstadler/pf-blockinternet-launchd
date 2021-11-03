A bash script and `launchd` definition for enabling/disabling all internet access at certain times of the day.

### Installation

1. copy all files to `/Library/LaunchDaemons/`
2. `sudo launchctl load -w /Library/LaunchDaemons/blockinternet.plist`

Manually override time-based setting by calling one of

```bash
sudo /Library/LaunchDaemons/blockinternet on  # equivalent to pfctl -e
sudo /Library/LaunchDaemons/blockinternet off # equivalent to pfctl -d
```
