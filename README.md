## MULTI-LANGUAGE SYSTEM  ( SPIGOT & VELOCITY )

> // Create
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "hi-user"))
                .set(Language.ITALIAN, "Ciao %value%, come stai?")
                .set(Language.ENGLISH, "Hi %value%, how are you?")
                .build();
```

> // Get
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "hi-user"));
```

> // Send
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "hi-user"))
                .replace("%value%", "zHeroandre")
                .send(player);
```

----
