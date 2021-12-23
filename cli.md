---
description: How to use the command line interface (CLI) for Flutter Distributor
---

# CLI

## Installation

```
dart pub global activate flutter_distributor
```

## Commands

{% hint style="info" %}
These commands are sorted in alphabetical order. The most commonly used are  package, publish, and release.&#x20;
{% endhint %}

### Package

Will package your application into a platform specific format and put the result in a folder.

<table><thead><tr><th>Flag</th><th>Value</th><th data-type="checkbox">Required</th></tr></thead><tbody><tr><td><code>--platform</code></td><td>Platform, e.g. <code>android</code></td><td>true</td></tr><tr><td><code>--targets</code></td><td>Comma separated list of maker names</td><td>true</td></tr></tbody></table>

Example:

```
flutter_distributor package --platform=android --targets=aab,apk
```

### Publish

<table><thead><tr><th>Flag</th><th>Value</th><th data-type="checkbox">Required</th></tr></thead><tbody><tr><td><code>--path</code></td><td>Path, e.g. <code>dist/1.0.0+1/hello_world-1.0.0+1-android.apk</code></td><td>true</td></tr><tr><td><code>--targets</code></td><td>Comma separated list of maker publishers</td><td>true</td></tr></tbody></table>

Example:

```
flutter_distributor publish --path dist/1.0.0+1/hello_world-1.0.0+1-android.apk --targets fir,pgyer
```
