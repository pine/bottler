# Bottler &nbsp;[![Build Status](https://travis-ci.org/emoji-gen/bottler.svg?branch=master)](https://travis-ci.org/emoji-gen/bottler)

:cookie: Cookie serializer and deserializer library for Java.

## Getting Started
TODO

## Usage

```java
CookieManager manager = CookieManager.getInstance();
CookieStore store = manager.getCookieStore();

ByteArrayOutputStream os = new ByteArrayOutputStream();
CookieStoreUtils.writeTo(store, os); // Save!

store.removeAll();

ByteArrayInputStream is = new ByteArrayInputStream(os.toByteArray());
CookieStoreUtils.readFrom(store, is); // Restore!!
```

## Test

```
$ ./gradlew clean test
```

## License
MIT &copy; [Emoji Generator](https://emoji.pine.moe/)
