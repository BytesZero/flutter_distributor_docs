# exe

## Usage

Add `make_config.yaml` to your project `windows/packaging/exe` directory.

```yaml
// The value of AppId uniquely identifies this application. 
// Do not use the same AppId value in installers for other applications.
appId: 5B599538-42B1-4826-A479-AF079F21A65D
appPublisher: LeanFlutter
appPublisherUrl: https://github.com/leanflutter/flutter_distributor
```

Run:

```
flutter_distributor package --platform windows --targets exe
```
