## MULTI-LANGUAGE SYSTEM

> // Create
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "no-player"))
                .set(Language.ITALIAN, "Ciao %value%, come stai?")
                .set(Language.ENGLISH, "Hi %value%, how are you?")
                .build();
```

> // Get
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "no-player"));
```

> // Send
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "no-player"))
                .replace("%value%", "zHeroandre")
                .send(player);
```

----
