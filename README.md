## MULTI-LANGUAGE SYSTEM  (SPIGOT & VELOCITY)

Use the `build()` method only if you want to cache the message, if you don't use it you won't be able to get this message anymore.
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "hi-user"))
                .set(Language.ITALIAN, "Ciao %value%, come stai?")
                .set(Language.ENGLISH, "Hi %value%, how are you?")
                .build();
```

If the multi-language message does not exist it will create one with that identifier.
$~$
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "hi-user"));
```

// Send
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "hi-user"))
                .replace("%value%", "zHeroandre")
                .send(player);
```

----
