# Instagram Agent Skills

14 Claude skills for running an Instagram account: planning, scripting, captions, publishing, engagement and analytics. MIT licensed.

## Skills

| Skill | What it does |
|---|---|
| `/ig-reel` | Write a complete Instagram Reel draft: 3 scored hooks, script, on-screen text and beat sheet. |
| `/ig-viral` | Find what makes Reels go viral in the user's niche and adapt the pattern into original ideas. |
| `/ig-caption` | Write Instagram captions with a strong first line that survives the '... |
| `/ig-carousel` | Plan and write a swipeable Instagram carousel: slide-by-slide copy, visual direction and caption. |
| `/ig-story` | Create an Instagram Story sequence with stickers, polls and a clear flow. |
| `/ig-profile` | Score an Instagram profile (bio, name field, highlights, grid, link) and rewrite the weak parts. |
| `/ig-plan` | Build a weekly Instagram content calendar with post types, times, topics and accounts to engage with. |
| `/ig-publish` | Publish or schedule an approved Instagram post, Reel, carousel or story after explicit confirmation. |
| `/ig-audit` | Audit an Instagram account's last 30 days: what worked, what failed, and what to change. |
| `/ig-research` | Research a niche: rank competitors' and peers' Reels against each account's own baseline, and find topic gaps. |
| `/ig-comment` | Draft thoughtful comments for other creators' posts to grow reach and relationships. |
| `/ig-reply` | Draft replies to comments on the user's own posts, in their voice, and flag spam, questions and leads. |
| `/ig-dm` | Set up comment-to-DM automations and write DM reply flows. |
| `/ig-analytics` | Read and explain Instagram analytics: reach, retention, saves, shares, follower growth and best posting times. |

## Install

**Claude (claude.ai / app):** zip a skill folder (for example `skills/ig-reel`) and upload it under Settings, Capabilities, Skills. Repeat per skill.

**Claude Code:** copy the folders in `skills/` into `~/.claude/skills/` (or `.claude/skills/` in a project). Or open Claude Code in this repo and say: "Install every skill in ./skills".

## First run

1. Run `/ig-profile`. It asks a few questions and creates `data/account.md`.
2. Run `/ig-research` and `/ig-plan` to get a week of content.
3. Run `/ig-reel`, `/ig-carousel`, `/ig-caption` for each slot.
4. Run `/ig-publish` to post. It always asks for confirmation first.

## Publishing and automation

Publishing, comment replies and DM automations need an Instagram connector: the official Instagram Graph API or a scheduling tool that wraps it. Connect one in your Claude setup. Without a connector, every skill still works and `/ig-publish` outputs a copy-ready manual posting package.

## Safety

- Nothing is published, commented or sent without your explicit yes.
- Use only the official Instagram API. No scraping, no bulk follow or like bots.
- Comment-to-DM flows must include an opt-out and only message people who interacted.

## Structure

```
skills/<name>/SKILL.md   one folder per skill
shared/                  hook formulas and style rules
data/                    your account profile, plans and logs (keep private)
```
