```ts
commands.raw('lolli', async function (message) {
  await message.addReaction(discord.decor.Emojis.LOLLIPOP);
  // Alternatively use `🍭`, this is much cleaner though
});
```
