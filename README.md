```
🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦
🟦🟦😁🟦🟦🟦😁🟦🟦🟦😁🟦🟦🟦😁😁😁🟦😁😁😁🟦😁😁😁😁🟦😁🟦🟦🟦😁🟦🟦
🟦🟦😁😁🟦😁😁🟦🟦😁🟦😁🟦🟦🟦🟦😁🟦🟦😁🟦🟦😁🟦🟦🟦🟦🟦😁🟦😁🟦🟦🟦
🟦🟦😁🟦😁🟦😁🟦😁🟦🙄🟦😁🟦🟦🟦😁🟦🟦😁🟦🟦😁😁😁🟦🟦🟦🟦😁🟦🟦🟦🟦
🟦🟦😁🟦🟦🟦😁🟦🟦😁🟦😁🟦🟦😁🟦😁🟦🟦😁🟦🟦😁🟦🟦🟦🟦🟦🟦😁🟦🟦🟦🟦
🟦🟦😁🟦🟦🟦😁🟦🟦🟦😁🟦🟦🟦🟦😁🟦🟦😁😁😁🟦😁🟦🟦🟦🟦🟦🟦😁🟦🟦🟦🟦
🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦
```

# Mojification

**Mojification** is a Jupyter Notebook-based helper for alignment of two texts in different languages. Based on [Lingtrain Aligner](https://github.com/averkij/lingtrain-aligner) (version 0.8.7), it does not change texts, but “mojifies” them.

>🤓 **to mojify** *verb* /ˈmɒdʒɪfaɪ/ to wrap corresponding sentences of two texts in different languages in emoji

Example of two mojified paragraphs from [“Le Petit Prince” / “The Little Prince”](https://bilinguator.com/book?book=le_petit_prince):

>🦊– Les hommes ont oublié cette vérité, dit le renard.🦊 💭Mais tu ne dois pas l’oublier.💭 ⏳Tu deviens responsable pour toujours de ce que tu as apprivoisé.⏳ 🌹Tu es responsable de ta rose…🌹
---
>🦊“Men have forgotten this truth,” said the fox.🦊 💭“But you must not forget it.💭 ⏳You become responsible, forever, for what you have tamed.⏳ 🌹You are responsible for your rose…”🌹

It’s used only to help to detect corresponding sentences while manually aligning two texts, for example, with the help of [B-Editor](https://github.com/bilinguator/b-editor) or other aligner. The order of sentences is not violated in this case.

## Five simple steps to mojify your text

1. Load packages
2. Load two texts
3. Align
4. Mojify texts
5. Save mojified texts

Emojis used in mojufication are symbols not presented in both texts. During every modification the set of used emojis are saved to file in the [emojis](emojis) folder and deleted in de-mojification step.

## Three simple steps to de-mojify your text 

>🤓 **to de-mojify** *verb* /ˌdiːˈmɒdʒɪfaɪ/ to delete emojis from two aligned texts

When two texts have been aligned, there is need to remove all emojis from them. Three steps to do it:

1. Load packages
2. Load two texts
6. De-mojify texts
