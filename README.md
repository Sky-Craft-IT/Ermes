> 即更长的单词或短语的缩写形式，前提是开启识别HTML标签时，已默认开启
> fewf3erfrefrefrefref

```java
LanguageBuilder.language(LanguageBuilder.identifier(this, "no-player"))
                .set(Language.ITALIAN, "Questo player non è stato trovato.")
                .set(Language.ENGLISH, "This player was not found.")
                .build();
```
