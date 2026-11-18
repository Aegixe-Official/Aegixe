# Using AegixeBot for public-address risk checks

[中文](telegram-bot-guide.zh-CN.md)

Historical reference dated 27 October 2026. Current workflow, fees, limits and network coverage have not been reverified. Follow the bot's current instructions. For a checked web workflow, see the [address risk detection guide](wallet-address-risk.md).

## Private chat

1. Open [AegixeBot](https://t.me/AegixeBot) and verify the exact username, `@AegixeBot`.
2. Select Start and read the instructions; use `/start` when needed.
3. Send a complete public address and select or specify the actual network as instructed.
4. Match the reply to the address, network and time before reading risk details.

Do not send private keys, recovery phrases, login codes or recovery files.

## Group chat

Where the bot is already available, mention it and include the complete public address in the same message:

```text
@AegixeBot <complete public address>
```

Replace the explanatory placeholder with the actual address. Follow current instructions if a network must be specified. Group administrators should grant permissions according to actual requirements; administrator access is not a universal prerequisite.

Other members may see the message and result. Use private chat when group disclosure is unsuitable; private chat still sends the submitted information to the bot service.

## Interpret the result

A warning needs investigation. No warning only describes the check's data coverage and time. An error or missing result remains unknown. Scores are not loss probabilities, and associations do not establish wrongdoing or a current issuer freeze. Exchange acceptance is a separate question.

[Web address checker](https://risk.aegixe.com/) · [AEGIXE website](https://aegixe.com/)




Updated 12 November 2026. See [sources and review status](../SOURCES.md) for scope.
