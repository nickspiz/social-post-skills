---
name: bluesky-post
description: Write, review or plan a Bluesky post or reply. Use when the target network is Bluesky, especially when the same idea was already written for X, because Bluesky needs a rewrite and not a copy.
---

# Bluesky post

Read `post-basics` first. It covers facts, the invented-claims guard, topic mix, timing and the final checklist.

## When to use

A post or reply for Bluesky. If a version for X already exists, this skill is how you make the second one.

## Rewrite, do not copy

Do not post the same text on X and Bluesky. Readers who follow you on both see it twice, and it looks like a cross-poster. Take the same fact and write a new post:

- change the opening and the ending;
- change the shape (if the X post was an opinion, make the Bluesky one a question or a small observation);
- change the length when it makes sense;
- keep every fact exactly the same. A rewrite changes wording, never claims.

If the idea is weak enough that you can only change words and not the shape, skip Bluesky that day.

## Voice

A bit slower and more conversational than X. The audience tends to read replies and reward a clear, kind tone. No rage bait, no hashtags, no sarcasm for effect.

## Form

- Limit: 300 graphemes (visual characters) per post. Aim well under. Some posts are one sentence. The limit counts graphemes, so an emoji built from several code points counts as one.
- Plain text. No Unicode "bold" letters. Emoji: at most one.
- Links are rendered as cards, so a link can sit at the end. Use one only when it is the point.
- Hashtags: skip.
- Rotate formats the same way as on X, but not in the same order on the same day.

## Images

- Up to 4 images per post (images and video cannot be combined). Alt text is expected here, and people notice when it is missing. Describe what is actually on the picture.
- Personal account: plain real screenshot. Brand account: designed image with real product UI. See `post-basics`, section 6.
- An image is fine on every post when you have a good one. Do not force it.

## Replies

Same rules as on X: live threads only, real experience only, specific and short. Bluesky has strong custom feeds and small communities, so a reply that adds something is remembered.

## Example

X version, from the `x-post` example:

> Saved carts are live in Pinecone Shop. Close the tab, come back tomorrow, the cart is still there.

Bluesky rewrite:

> Small change in Pinecone Shop this week: the cart now survives a closed tab. Handy if your customers like to sleep on a purchase.

Same single fact (saved carts), new shape. "Handy if..." is a framing, not a new claim. Check that it stays one.

Checked 11.10.2026: https://github.com/bluesky-social/atproto/blob/main/lexicons/app/bsky/feed/post.json (300 graphemes), https://github.com/bluesky-social/atproto/blob/main/lexicons/app/bsky/embed/images.json (up to 4 images; an embed is one of images, video, external or record)
