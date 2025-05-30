# 📦ZipSigner

**ZipSigner** is an open-source Java command-line tool for signing Android APKs and JAR files.
- Extracted from the signing utilities in old [Magisk](https://github.com/topjohnwu/Magisk) versions. 

- Built for JDK 8+ with Bouncy Castle 1.80

## Build

Using Gradle to build the executable JAR:

```bash
./gradlew jar
```

## Usage

1. Sign with AOSP Test Keys
```bash
java -jar zipsigner.jar input.apk output.apk
```

2. Sign with Certificate and Private Key
```bash
java -jar zipsigner.jar x509.pem pk8 input.apk output.apk
```

3. Sign with Java KeyStore
```bash
java -jar zipsigner.jar keyStore keyStorePass alias keyPass input.jar output.jar
```

## Credits
- [**BlassGO**](https://github.com/BlassGO): Creator of this ZipSigner variant
- [**topjohnwu**](https://github.com/topjohnwu) & [**osm0sis**](https://github.com/osm0sis): I based this on their [ZipSigner](https://github.com/Magisk-Modules-Repo/zipsigner) for Android.