# nfa
A Go command line app to send notifications to [Notifications for Android TV](https://play.google.com/store/apps/details?id=de.cyberdream.androidtv.notifications.google&hl=en) / [Notifications for Fire TV](https://play.google.com/store/apps/details?id=de.cyberdream.firenotifications.google&hl=en)

# Instructions
1. `go get github.com/robbiet480/nfa`
2. `$GOPATH/bin/nfa`

# Usage
```
Sends a notification to Notifications for Android TV/Notifications for Fire TV.

Usage:
  nfa notify [flags]

Flags:
  -a, --address ip                IP Address Notifications for Android TV or Notifications for Fire TV is running on.
  -n, --app-name string           App name to display the notification as generated by (default "nfa.go")
  -b, --background-color string   Background color of the notification, given in hex format. (default "#607d8b")
  -d, --duration duration         The duration in seconds for which the notification will be displayed. (default 5s)
  -i, --icon string               Path to icon (default "/Users/robbiet480/gocode/src/github.com/robbiet480/nfa.go/gopher.png")
  -x, --interrupt                 If set, the notification is interactive and can be dismissed or selected to display more details. Depending on the running app (e.g. Netflix), this may stop playback.
  -m, --message string            Message to show (default "Hello from nfa.go!")
  -p, --port int                  Port to connect on (default 7676)
  -o, --position string           Position of the notification on screen. Must be one of bottom-right|bottom-left|top-right|top-left|center (default "bottom-right")
  -t, --title string              Title of notification (default "nfa.go")
  -s, --transparency string       Transparency percentage. Must be one of default|0%|25%|50%|75%|100%. (default "default")

Global Flags:
      --config string   config file (default is $HOME/.nfa.yaml)
```

# Contributing
1. Fork
2. Create branch
3. Create changes
4. Submit PR
5. ...
6. Profit

# Credits
gopher.png is from [here](https://github.com/golang-samples/gopher-vector).

# License
MIT
