
# Documentació del Bot de Discord

![Logotipo de Discord](https://img.magnific.com/vector-premium/discordia-logotipo-moderno_578229-177.jpg?semt=ais_hybrid&w=740&q=80)

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
