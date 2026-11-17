# home-robot

A personal robot that does housework at home: tidy the kitchen, do the
laundry, use the computer. This repo is the research log for getting
there — what exists today, what to build first, and a dated note each
time the daily research turns up something worth keeping.

Personal project, public sources only. No company code or data.

## The goal, concretely

- **Tidy the kitchen:** put things back where they belong, load the
  dishwasher, clear the counters.
- **Laundry:** load the washer, take clothes out of the dryer, fold them.
- **Use the computer:** look up recipes, order groceries, keep lists.
  (A software agent does this better than a body — no arm needed.)

## Reality check (2026-11-17)

Ranked by difficulty, easiest first:

1. **Using the computer** — easiest, and bodiless. A software agent
   operating the computer directly beats a robot arm typing on a keyboard.
2. **Tidying the kitchen** — medium. "Move an object from A to B" is
   doable for Stretch/NEO-class hardware in a fixed scene; oily, wet,
   fragile, or stacked items are not.
3. **Laundry** — hardest. Washers and dryers are already automated; the
   robot's job is loading, unloading, and folding. Folding deformable
   cloth has demos, no reliable product.

Nothing on the market today can be bought and trusted with all three.

## Two paths

**Buy:** 1X NEO — $20,000 to own or $499/month, $200 refundable
deposit, US deliveries starting 2026. Ships with basic autonomy;
complex chores go through Expert Mode, i.e. a 1X operator remotely
piloting the robot. No independently verified home use yet.

**Build:** start from one chore. The most buildable first skill is
"pick up scattered objects and put them in a bin" — fixed-scene
grasping and placing. A desktop SO-101 arm is where that starts; a
mobile base comes later.

## Starter parts

| Part | Role | Price (Nov 2026) |
| --- | --- | --- |
| SO-101 arm pair (LeRobot default) | Manipulation | ~$230 parts; ¥1,343 in China; kits $199–$299 |
| Orbbec Gemini 335 | Depth camera (eyes) | ~¥1,950 |
| Laptop / Jetson Orin NX | Compute | Whatever you have; Jetson has no domestic clone |
| Unitree Go2 Air (later) | Mobile base | ¥8,997 on JD; ¥7,647 after subsidy |

Many of these parts are Chinese-made already: the SO-101's servos are
Feetech, its kits ship from Seeed / WowRobo / Hiwonder, and Unitree is
based in Hangzhou.

## Why there is no big unified platform (yet)

No standard body (every task wants a different one), no volume (parts
ship in thousands, not hundreds of millions), safety/liability (a
wrong move breaks things or hurts people), and the software layer is
newborn — VLA models only took off after 2024. Willow Garage's PR2 and
Google's Everyday Robots both tried and shut down. What is changing:
the humanoid is becoming the default body (homes are built for human
bodies), and VLA models may become the unifying layer.

## Research log

Dated notes live in `research/`. A new note is added whenever the daily
research turns up something notable — a new capability, a new failure
mode, a price move, or a decision-changing benchmark. No padding.

## Companion

- Notion project page (personal tracking + research database):
  <https://app.notion.com/p/41bc2976d61e815ea734e4ede33ef112>
