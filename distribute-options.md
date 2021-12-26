# Distribute Options

## Example

```yaml
env:
  FIR_API_TOKEN: 'your api token'
  PGYER_API_KEY: 'your api key'
output: dist/
releases:
  - name: dev
    jobs:
      - name: release-dev-android
        package:
          platform: android
          target: apk
          build_args:
            target: lib/main.dart
            flavor: dev
            target-platform: android-arm,android-arm64
        publish_to: fir
      - name: release-dev-ios
        package:
          platform: ios
          target: ipa
          build_args:
            target: lib/main.dart
            flavor: dev
            export-options-plist: ios/dev_ExportOptions.plist
        publish_to: fir
```

## Specification <a href="#specification" id="specification"></a>

| Field Name | Type      | Description            |
| ---------- | --------- | ---------------------- |
| `env`      | `map`     | environment variables. |
| `output`   | `string`  | e.g. `dist/`           |
| `releases` |           |                        |

