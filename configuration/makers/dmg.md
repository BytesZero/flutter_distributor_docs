# dmg

{% hint style="warning" %}
You can only build the DMG target on macOS machines.
{% endhint %}

## **Requirements**

* `appdmg`

Run the following command

```
npm install -g appdmg
```

## Usage

Add `make_config.yaml` to your project `macos/packaging/dmg` directory.

```yaml
title: hello_world
contents:
  - x: 448
    y: 344
    type: link
    path: "/Applications"
  - x: 192
    y: 344
    type: file
    path: hello_world.app
```

Run:

```
flutter_distributor package --platform macos --targets dmg
```

## Related Links

[https://github.com/LinusU/node-appdmg](https://github.com/LinusU/node-appdmg)
