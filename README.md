## HANDLER SYSTEM

##

##

##

----

##

## MULTI-LANGUAGE SYSTEM  (SPIGOT & VELOCITY)

##

Example to create a multi-language message. <br />
Use the `build()` method only if you want to cache the message, if you don't use it you won't be able to get this message anymore.

```java
LanguageString message = LanguageBuilder.language(LanguageBuilder.identifier(ErmesMain, "hi-user"))
                .set(Language.ITALIAN, "Ciao %value%, come stai?")
                .set(Language.ENGLISH, "Hi %value%, how are you?")
                .build();
```

##

Example to take a multi-language message. <br />
If the multi-language message does not exist it will create one with that identifier.
```java
LanguageString message = LanguageBuilder.language(LanguageBuilder.identifier(ErmesMain, "hi-user"));
```

##

Example of how to send a multi-language message. <br />
You will be able to send messages to players via the `send()` method by passing them the parameter.
```java
LanguageString message = LanguageBuilder.language(LanguageBuilder.identifier(ErmesMain, "hi-user"))
                .replace("%value%", "zHeroandre")
                .send(player);
```

----
