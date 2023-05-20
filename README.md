# Flutter Amplify Template

This is a Flutter app template with AWS Amplify integration.

## Configure AWS Amplify

This project is a starting point for a Flutter application which uses AWS Amplify services.
In order to use it, you need to configure your serverless Amplify backend first
(e.g. via Amplify CLI).

The following commands are brief excerpts from the official documentation:
[Official Amplify (Flutter) documentation](https://docs.amplify.aws/start/q/integration/flutter/)

### Configure

This command configures the Amplify CLI and thus only must be executed once per
development device.

```amplify configure```

### Initialize

This command initializes the Amplify project within this Flutter project and
must be executed regardless of which specific Amplify capabilities you will use.

```amplify init```

### Various categories

This template assumes that you want to work with all Amplify categories which
are currently supported for Flutter.
These must all be added first:

```amplify add <category>```

(for DataStore also execute ```amplify codegen models```)

For each Amplify capability that you do **not** want to use, please remove the
respective plugin from following files (look out for TODO comments):
- [my_app.dart](lib/my_app.dart)
- [pubspec.yaml](pubspec.yaml)
