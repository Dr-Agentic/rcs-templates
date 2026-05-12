# RCS Business Messaging Templates

Production-ready JSON templates for RCS (Rich Communication Services) Business Messaging. GSMA Universal Profile compliant.

## Free Templates

| # | Template | Description |
|---|---|---|
| 1 | [Text + Suggested Actions](templates/01-text-suggestions.json) | Quick-reply buttons for user interaction |
| 2 | [Rich Card (Vertical)](templates/02-richcard-vertical.json) | Image + title + description + buttons |
| 3 | [Carousel (2 Cards)](templates/03-carousel-2.json) | Swipeable card layout |
| 4 | [Calendar Action](templates/04-calendar-action.json) | Add-to-calendar from message |
| 5 | [Suggested Reply](templates/05-suggested-reply.json) | Lightweight reply chips |

## Quick Start

1. Copy a template
2. Customize the content
3. Test on [RCS X](https://rcsxplatform.net) (free emulator)
4. Submit to carrier

## Validation Checklist

Before carrier submission, verify:

- `contentMessage` wrapper present
- Valid JSON (no trailing commas)
- Text ≤ 3072 characters, UTF-8
- `cardOrientation` is VERTICAL or HORIZONTAL (rich cards)
- Title ≤ 200 chars, Description ≤ 2000 chars
- Media height: SHORT, MEDIUM, or TALL
- `fileUrl` uses HTTPS
- Image max 3.5MB JPEG, 1MB PNG
- Max 4 suggestions per message
- Suggestion text ≤ 25 chars
- `postbackData` ≤ 200 chars

## Want More?

The **[RCS Developer Starter Kit](https://rcsxplatform.net)** includes:

- 15+ production-ready templates (including video cards, multi-message, AI agent formats)
- Complete GSMA validation checklist
- SMS-to-RCS migration playbook
- MCP server integration patterns
- Carrier approval guide (US/EU/APAC)
- Testing matrix

## Test Free

[RCS X](https://rcsxplatform.net) — Professional RCS emulator. No carrier agreements needed.

## License

MIT
