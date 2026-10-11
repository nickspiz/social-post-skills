# social-post-skills

**Skills for Claude Code that describe how to write, pick and check posts for each social network.**

![License: MIT](https://img.shields.io/badge/license-MIT-green)
![Works with Claude Code](https://img.shields.io/badge/works%20with-Claude%20Code-d97757)

I'm not a developer. I build products with Claude Code, and part of running a product is posting about it: LinkedIn, X, Bluesky, Threads, Instagram, Telegram, Reddit. Every network wants something a little different, and I kept being corrected on the same things: a number that wasn't real, a story that didn't happen, the same post told twice in one week, a Telegram message that read like a LinkedIn one.

So I wrote the corrections down as skills. This repo is that list, cleaned up so it works for any small founder.

## What's inside

One shared skill with the rules that hold everywhere, and one skill per network.

| Skill | What it covers |
|---|---|
| `post-basics` | Facts, the invented-claims guard, topic mix, variety, replies, timing, images, final checklist |
| `linkedin-post` | The first two lines, length, documents and images, personal profile versus company page |
| `x-post` | Short form, no Unicode bold, alternating images, replies, threads |
| `bluesky-post` | Why it is a rewrite and not a copy of the X post, alt text, links |
| `threads-post` | Its own text, short posts, images on brand accounts |
| `instagram-post` | Picture first, carousels, captions |
| `telegram-post` | Emoji, HTML bold and italic, caption limits, alert format |
| `reddit-post` | First post is an intro, founder style, links rarely, community rules |

## The rules I care about most

- Every number and claim comes from a facts list you provide. If it isn't on the list, it doesn't go in the post.
- No invented experience. No "I've watched this fail", no "people keep asking me".
- No rumours. A Reddit thread is not a source. "Is testing" never becomes "rolled out".
- About 75-80% of posts are about your own product. A competitor or trend post at most once in four or five, with your own angle.
- Weak numbers stay out. A post without a number is fine.
- Different lengths. Some posts are one sentence.
- Bluesky is a rewrite, Threads is its own text.
- Brand images use real product UI, designed for the post. A personal account gets a plain screenshot.

## Before and after

A draft with no guard:

> Saved carts are live in Pinecone Shop. We built it because most shoppers left at checkout. Merchants tell us conversion is up 20%.

With the skills, given only one fact (`Saved carts shipped 3 March, source: changelog`):

> Saved carts are live in Pinecone Shop. Close the tab, come back tomorrow, the cart is still there.

The reason and the 20% were never in the facts, so they are gone. (Pinecone Shop is a made-up example.)

## Install

As a Claude Code plugin:

```text
/plugin marketplace add nickspiz/social-post-skills
/plugin install social-post-skills@social-post-skills
```

Or copy the folders you need into your project:

```bash
git clone https://github.com/nickspiz/social-post-skills
cp -r social-post-skills/skills/post-basics social-post-skills/skills/x-post .claude/skills/
```

Always install `post-basics` together with a network skill. The network skills point to it.

## Use it

Give Claude a facts list and a voice sample, then ask:

- "Write a LinkedIn post about saved carts. Facts are in facts.md."
- "Rewrite this X post for Bluesky."
- "Check these five drafts against post-basics and tell me what fails."

The skills load by themselves when the task matches.

## The final pass

The skills end with a human-writing check. The checklist they point to is [blader/humanizer](https://github.com/blader/humanizer) (MIT). It is a separate project, so install it yourself if you want it.

## Limits and formatting change

Character limits and features differ between networks and change over time. The numbers in the skills were checked against official platform documentation on 11.10.2026; where a number could not be confirmed there, the skill tells you to check the platform's help instead. If one is wrong or out of date, please open an issue with a link to the platform's documentation.

## Questions and ideas

Have a question or an idea? Start a [discussion](https://github.com/nickspiz/social-post-skills/discussions). For mistakes, open an [issue](https://github.com/nickspiz/social-post-skills/issues/new/choose). See [CONTRIBUTING.md](CONTRIBUTING.md) before sending a pull request.

## Privacy

The plugin is plain-text skills. It has no scripts and no hooks. The plugin itself reads no files, calls nothing and makes no network requests. It writes nothing and sends nothing to the author. It only changes how Claude writes and checks posts. Whatever Claude does afterwards happens through the tools and permissions you already have in your session.

## Support

Questions or bugs: [GitHub Issues](https://github.com/nickspiz/social-post-skills/issues) or hello@nickspiz.com.

## License

MIT. See [LICENSE](LICENSE).
