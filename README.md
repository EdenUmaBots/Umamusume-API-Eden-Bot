## Icarus v2.0 — The Big One

__The biggest leap since launch. The Trackblazer Engine grows up: it chases set-bonuses, races smarter without over-racing, spends the shop like a pro, picks event answers from a 3,600+ event database — and the dashboard finally shows you what it's doing, item icons and all. Here's everything new__

## ⚙️ The Trackblazer Engine is now the default
A **solver-driven decision core** built for the Trackblazer/MANT scenario. Instead of scoring one turn at a time, it treats your **whole career as a single optimization problem**:
- 🗓️ **Whole-career race scheduling** — an exact route optimizer (with a fast heuristic fallback) weighs the entire calendar at once and locks in the schedule that maximizes stats, fans, set-bonus completion and aptitude fit — while respecting your max-races-in-a-row limit and the summer/finale windows.
- ♻️ **Plans, then adapts** — solved at career start, then re-planned live when a race is lost or drops off the calendar, so it stays valid as the run actually plays out.
- 🏁 **Built around the racing economy** — train-vs-race-vs-rest decisions account for the currency → items → stats loop, energy, mood, consecutive-race risk, and the marquee G1s & finale climax races.
- 🛡️ **Smarter, safer racing** — energy/streak guards, a marquee-race prediction gate, and summer/finale handling push for value without over-racing or throwing winnable races.
- 🔁 **Classic is still here** — the previous turn-by-turn engine is one click away under *Decision Engine* __Classic is still here__ — the previous turn-by-turn engine is one click away under Decision Engine.

## 🏆 Race & Set-Bonus Engine
- 🥇 **Chases set-bonuses (Epithets)** — new *Chase Achievable Set-Bonuses* option: the Smart Race Solver now schedules races to **complete sets** — Triple Crowns, distance/regional/surface sets and more — for their large random-stat rewards that were previously left on the table. This is the headline stat lever.
- ♻️ **Live Schedule Re-Planning toggle** — a proper switch in Smart Race Solver settings: ON (default) re-routes the remaining schedule after a loss; OFF locks in the plan solved at career start.
- 🚫 **No more over-racing** — a runtime cap now honors your *max races in a row* setting. Careers that ran 46–48 races with 8–10 in a row now run ~42 with streaks capped — recovering total stats and win rate.
- 🎯 **More marquee G1s run** — fixed race matching for marquee races (Japan Cup, Arima Kinen, Takarazuka Kinen, Tenno Sho…) that the game offers under several internal IDs. They were being skipped; now they run.
- ⚖️ **Outcome Risk has its own section** in Racing settings, with a toggle — you decide whether the solver weighs race-loss risk.

## Stat Focus

__New Stat Focus control: Balanced spreads stats evenly, while Capped concentrates your priority stats to push their ceilings. Set it per preset.__

## Speed

__The old Tempt-Fate on/off toggle is replaced by a Speed dropdown — Safe / Fast / Faster / Ludicrous. The levels now genuinely differ: each scales the bot's pacing (Safe keeps human-like timing; Ludicrous removes it). Previously Fast, Faster and Ludicrous all ran at the same real speed — fixed.__

## Shop & Items
- Smarter shop spending — race hammers are conserved and saved for the three finale climax races (where they pay off most); training megaphones & anklets are bought for your priority stats; energy, cures and snacks are bought by need; and a finale coin reserve keeps funds on hand for the climax.,
- Item icons in Decision Reasoning — every shop item the bot buys or uses now shows its in-game icon beside its name.

## Event Choices
The event auto-selector got a major upgrade:

- Massively expanded coverage — when there's no observed data for an event, it now falls back to a 3,600+ event effect database and scores the real choice effects, instead of a blind "pick the second option" guess.,
- Stat-cap aware — no longer over-values points dumped into an already-maxed stat.,
- Turn-aware energy — values energy more during summer camp and the finale stretch, where it matters most.,
- More accurate matching — tightened event lookup so it won't mis-score an unrelated event that merely shared a few trailing ID digits.

## Decision Reasoning

__Clearer, more accurate per-turn explanations — including correct item labels (training megaphones shown as training boosts, race hammers as race buffs) so the panel matches what actually happened. The live on-screen race list is now captured for diagnostics too.__

## Fixes & Quality of Life

- Career History sparks are correct per career — each finished career now shows the sparks it actually earned, instead of repeating the same inherited parent sparks every time.
- Running style is set correctly (e.g. Oguri Cap runs Pace, not Late) — fixed the in-race running-style change to send the right data at the right step.
- Skill-config UI fixes and a fixed dashboard console/network error.

-------------

## Join our discord: https://discord.gg/wpbd3hTBDc

-------------

# ! Written installation guide, video below.

You will need the latest version of python and C++ Build Tools:

https://www.python.org/downloads/

https://visualstudio.microsoft.com/visual-cpp-build-tools/

For C++ Tools, this is what you need, just check that box. <img width="1221" height="625" alt="image" src="https://github.com/user-attachments/assets/28610cb3-650d-43c9-bf09-4505a62272de" />

# First time instalation:

Step 1: Download bot directly from this repo, unzip file

Step 2: Open the bot folder (usually second one) in cmd like this, please note, this is an example link, yours will be different.

```cmd
cd C:\Users\yourusernamehere\Downloads\Umamusume-API-Bot-main\Umamusume-API-Bot-main
```
Step 3: Paste the following lines in order. 

```cmd
winget install -e --id OpenJS.NodeJS
```
Accept terms, then:

```cmd
npm i
```
Disregard the error you might have here, then:

```cmd
pip install -r requirements.txt 
```
Once the above it done, paste or type:

```cmd
python main.py
```

The bot will launch steam and umamusume then promptly close the game shortly before fully loading in, you will be given a web address, please paste this into your browser, you will be promted to log into your steam account, (it is recommended to use an alt). Web UI will request a steamguard code, once provided, you're in! Everything from here should be self explanitory. 

# Video Guide: https://www.youtube.com/watch?v=SkBItJYJMeE

# Regular use:


```cmd
cd C:\Users\yourusernamehere\Downloads\Umamusume-API-Bot-main\Umamusume-API-Bot-main
```

```cmd
python main.py
```


# Running multiple bots!

Ensure you have multiple seperate folders and keep track. Each bot must have it's own port number, this is located in main.py, line 186, change it to something else, default is 1200, so second bot could be 1201. Each bot needs its own steam account.

Launch first bot until you're in web UI, switch steam accounts, repeat the process. Turn on each bot simoultaneously. First bot acts as an anchor, if this crashes, all bots will crash. We found that we were able to comfortably run 3 accounts at the same time, could try more.

Daily reset will cause the bots to crash, you must set everything up manually then. 

# Future updates.

We will be working towards updating the bot as we see fit and will be porting it over to new scenarios, if you would like to contribute, get in touch with us though discord. Clank responsibly and thank you all. 













