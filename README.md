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

> // Send  (org.bukkit.command.CommandSender, org.bukkit.entity.Player, com.velocitypowered.api.command.CommandSource, com.velocitypowered.api.proxy.connection.Player)
```java
LanguageString languageString = LanguageBuilder.language(LanguageBuilder.identifier(this, "no-player"))
                .replace("%value%", "zHeroandre")
                .send(player);
```

----
