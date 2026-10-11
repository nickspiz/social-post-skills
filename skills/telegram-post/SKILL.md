---
name: telegram-post
description: Write, review or plan a post for a Telegram channel or group of a product or a founder. Use when the target is Telegram, including formatting with HTML (bold, italic, links) and captions on images.
---

# Telegram post

Read `post-basics` first. It covers facts, the invented-claims guard, topic mix, timing and the final checklist.

## When to use

A channel post, or an announcement in a community group. Telegram is the liveliest place of all the networks here. Readers subscribed on purpose, so you can be warmer and richer than elsewhere.

## Voice

Friendly, direct, a little more energetic than elsewhere. Brand channel: "we". Personal channel: "I". Still no invented experience and no hype words.

## Form

- **Emoji are welcome.** Several per post is normal: at the start of paragraphs, or as list markers. Keep them meaningful, not decoration for its own sake.
- **Bold and italic for emphasis.** Use HTML parse mode, because it needs less escaping than Markdown. Tags: `<b>`, `<i>`, `<u>`, `<s>`, `<a href="...">`, `<code>`, `<pre>`, `<blockquote>`.
- Escape `<`, `>` and `&` in plain text as `&lt;`, `&gt;` and `&amp;`, or the message will be rejected.
- Short paragraphs, one blank line between them.
- Length: a message holds up to 4096 characters. A caption under an image holds far less (1024 in the Bot API; check Telegram for the in-app limit), so count first. Most posts should be a screen or less.
- Rotate formats: a list of picks, a mini guide in steps, an opinion on confirmed news, a question to subscribers, before and after, a screenshot with a short breakdown.
- A short link preview is fine. Do not post three links in a row.

## Images

- Brand channel: designed picture with real product UI. Personal channel: plain real screenshot. See `post-basics`, section 6.
- If the image is optional for the format, a text post is fine.
- Do not write "see the picture above" unless the picture is attached.

## Topics

Mostly the product, how to use it, what changed and why. Subscribers expect release notes, small tips and honest behind-the-scenes. Competitor or trend posts at most 1 in 4-5, confirmed sources only.

## Frequency and timing

Weekdays, inside the daily window. A channel does not need a post every day. One good post beats three filler ones. Do not repeat on Telegram the same story you told on other networks the same day: give subscribers the extra detail instead.

## Notifications

If you send alerts through a bot (new release, incident), keep the format identical every time: one emoji and a bold headline, a blank line, then `<b>Label:</b> value` lines. No emoji inside the lines, no timestamp in the text, because Telegram shows one.

## Example

Facts: "Pinecone Shop saved carts, shipped 3 March. Works on the web and the app (changelog)."

```html
🛒 <b>Saved carts are here</b>

Close the tab, come back tomorrow, the cart is still there.

✅ Web
✅ App

Details in the <a href="https://example.com/changelog">changelog</a>.
```

Checked 11.10.2026: https://core.telegram.org/bots/api (4096 characters per message, 1024 per caption, supported HTML tags and escaping)
