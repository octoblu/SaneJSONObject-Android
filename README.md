# SaneJSONObject-Android

## Installation

- In library `build.gradle` add the dependency:

```gradle
dependencies {
    compile 'com.octoblu:sanejsonobject:4.0.1'
}
```

- jCenter will need to be in the repository list in the root project `build.gradle`

```gradle
buildscript {
    repositories {
        jcenter()
    }
    dependencies {
        // NOTE: Do not place your application dependencies here; they belong
        // in the individual module build.gradle files
    }
}

allprojects {
    repositories {
        jcenter()
    }
}
```

## Import

```java
import com.octoblu.sanejsonobject.SaneJSONObject;
```

## App Examples

* [BeaconBlu](https://github.com/octoblu/BeaconBlu-Android)
* [Gateblu](https://github.com/octoblu/gateblu-android)

## API

extends Android `JSONObject`

I am going to list the additional methods.

```java
public String getStringOrNull(@Nullable String name)
```

```java
public Integer getInteger(@Nullable String name, Integer value)
```

```java
public Boolean getBoolean(@Nullable String name, Boolean def)
```

```java
public Date getDateOrNull(@Nullable String name)
```

```java
public String getStringOrThrow(@Nullable String name)
```

```java
public SaneJSONObject getJSONOrNull(@Nullable String name)
```

```java
public void putOrIgnore(@Nullable String name, @Nullable String value)
```

```java
public void putBooleanOrIgnore(@Nullable String name, Boolean value)
```

```java
public void putIntOrIgnore(@Nullable String name, @Nullable Integer value)
```

```java
public void putDoubleOrIgnore(@Nullable String name, @Nullable Double value)
```

```java
public void putJSONOrIgnore(@Nullable String name, @Nullable JSONObject value)
```

```java
public void putArrayOrIgnore(@Nullable String name, @Nullable JSONArray value)
```

```java
public void putDateOrIgnore(@Nullable String name, @Nullable Date date)
```

```java
public static SaneJSONObject fromJSONObject(JSONObject data)
```

```java
public static SaneJSONObject fromString(String data)
```
