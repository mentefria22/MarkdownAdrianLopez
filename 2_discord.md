
# Documentació del Bot de Discord

![Logotip de Discord](https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/66e3d80b0c7a6f0e3c20f6b5_discord-logo.svg)

Pots registrar la teva aplicació al [Portal de Desenvolupadors de Discord](https://discord.com/developers/applications).

Per fer que el bot respongui, escoltem l'esdeveniment `messageCreate` i utilitzem el mètode `message.reply()`.

## Exemple de codi en JavaScript

Aquest exemple és molt senzill: quan algú escriu `ping`, el bot respon amb `pong!`. Així comprovem ràpidament que tot funciona.

```javascript
client.on('messageCreate', message => {
    if (message.content === 'ping') {
        message.reply('pong!');
    }
});
```
