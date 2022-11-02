# iOS-App-Info
The way to get information about the App.

### 1. App Product Name
-----------------
```
let appProductName = Bundle.main.object(forInfoDictionaryKey: "CFBundleDisplayName") as? String
```

### 2. iOS Verison
-----------------
```
let os = ProcessInfo.processInfo.operatingSystemVersion
print(String(os.majorVersion) + "." + String(os.minorVersion) + "." + String(os.patchVersion))
```
PRINT: 15.6.1

### 3. App Version
-----------------
```
let appVersion = Bundle.main.infoDictionary?["CFBundleShortVersionString"] as? String
print(appVersion)
```
PRINT: 1.0.1
