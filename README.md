-
> // Create
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "no-player"))
                .set(Language.ITALIAN, "Questo player non è stato trovato.")
                .set(Language.ENGLISH, "This player was not found.")
                .build();
```
-

--
> // Get
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "no-player"));
```
--
