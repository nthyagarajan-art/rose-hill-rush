# Rose Hill Rush

A Fordham-themed endless runner in the style of Subway Surfers. You're late for class and cutting through Fordham's Metro-North station, with a giant Ram mascot charging after you. Run the tracks, dodge Ram Vans, and grab as many Ram Coins as you can.

**Made by:** Neha Thyagarajan

**Play it in your browser:** https://nthyagarajan-art.github.io/rose-hill-rush/

## How to start the game

You don't need to install anything. The whole game is one file, `index.html`, and it runs in any modern browser (Chrome, Safari, Firefox, Edge) on a computer or a phone.

**Option 1: play online (easiest)**
Open the link above and click **START RUNNING**.

**Option 2: run it from this repository**
1. Click the green **Code** button on this page, choose **Download ZIP**, and unzip it. (Or clone it with `git clone https://github.com/nthyagarajan-art/rose-hill-rush.git`.)
2. Double-click `index.html` to open it in your browser.
3. Click **START RUNNING**, or press **Enter** or **Space**.

**Option 3: run it from a local web server (optional)**
If your browser blocks local files, run this from inside the project folder:
```
python3 -m http.server 8000
```
Then open http://localhost:8000 in your browser.

## Controls

| Action | Keyboard | Phone / touchscreen |
|---|---|---|
| Move left / right a lane | ← → (or A / D) | Swipe left / right |
| Jump | ↑ (or W / Space) | Swipe up |
| Slide / roll | ↓ (or S) | Swipe down |
| Pause / resume | P or Esc | Tap the ❚❚ button |
| Start / restart | Enter or Space | Tap the button |

Pressing ↓ while you're in the air slams you back down into a slide.

## Rules

- You run forward automatically along three tracks, and you get faster the farther you go.
- **Obstacles:** running into a van, barrier or banner ends your run (unless you have a shield).
  - **Ram Van:** too tall to jump. Switch lanes to get around it.
  - **Track-work barrier ("CLOSED"):** jump over it.
  - **Banner ("GO RAMS!", "HOMECOMING", …):** slide under it.
  - **Squirrel:** jump over it. If you hit one, you trip.
- **The Ram mascot:** he chases you at the start of every run. Tripping over a squirrel, or trying to switch into a lane that's blocked by something right beside you, counts as a **stumble**. The Ram then catches up and stays right behind you for about 7 seconds. **Stumble again while he's behind you and he head-butts you: game over.**
- **Ram Coins:** each one is worth 10 points.
- **Power-ups** (the glowing maroon circles):
  - 🧲 **Magnet:** pulls nearby coins to you for 10 seconds.
  - 🛡️ **Ram Shield:** absorbs one crash in the next 15 seconds.
  - 🍺 **Cold One:** doubles your score for 12 seconds.
- **Score:** you earn points for distance plus coins. Your best score is saved in your browser.

## Files

- `index.html`: the complete game (HTML, CSS and JavaScript). All graphics are drawn in code on an HTML canvas and all sounds are generated with the Web Audio API, so there are no separate image or sound files.
- `README.md`: this file.

## Notes

- Fan-made for a class project. Not affiliated with or endorsed by Fordham University.
- Built with help from Claude (Anthropic's AI assistant).
