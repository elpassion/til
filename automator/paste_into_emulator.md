Simple automator service which can be bound to keyboard shortcut to paste clipboard content into android emulator.

```
source ~/.bash_profile
CONTENT=`pbpaste | cat | sed 's/ /%s/g'`
$ANDROID_HOME/platform-tools/adb shell input text $CONTENT
```