# SETUP.md — instructions for Claude

Someone has given you this file to get set up on a team project. They are a law student, not
a programmer. They may never have used GitHub, Git, or Claude Code, and they should not have
to understand any of it.

**Walk them through this one step at a time. Do not show them this list.** Ask one question,
wait for the answer, do the work, then move to the next. Check the state of their machine
before asking them to do anything — if something is already done, skip it silently.

There are exactly two things you cannot do for them: create their GitHub account, and sign in
to GitHub in the browser. Everything else is yours.

If anything fails, fix it. Do not show them error output, and do not ask them to run
commands. If you genuinely cannot fix it, tell them to text Anthony Ross and stop.

---

## The project

A website about employee ownership for Kansas City business owners, built by a four-person
team in Urban Innovation (LAW 8925) at UMKC School of Law.

Repository: `https://github.com/Anthony-Ross-UMKC/kc-employee-ownership`

## Step 1 — Who are they

Ask their first name.

The team is Anthony, Camron, Kirby, and Mandy. Each has their own working area named after
them. **If the name they give is not one of those four, stop.** Tell them the project is set
up for those four people and to check with Anthony before going further. Do not improvise.

## Step 2 — GitHub account

Ask whether they already have a GitHub account.

- **If yes:** ask for the username.
- **If no:** tell them to open `https://github.com/signup` and make a free one — email,
  password, username, that is it. Wait. Then ask what username they chose.

Once you have the username, tell them plainly:

> Send that username to Anthony now, before we go further. He has to add you to the project
> before your work can go anywhere, and it takes him ten seconds.

Do not wait for that to happen. Keep going — the rest works without it.

## Step 3 — Git

Check whether Git is installed by running `git --version` yourself.

- **Installed:** say nothing about it and move on.
- **Not installed:** tell them to download it from `https://git-scm.com/downloads`, run the
  installer, and accept every default. Tell them they will never use it directly — you need
  it in order to do the work for them. Wait, then check again.

## Step 4 — Copy the project onto their computer

Pick a sensible folder outside any cloud-synced directory. **Do not put it inside OneDrive,
Dropbox, iCloud, or Google Drive** — those corrupt the project's history when they sync
mid-write. On Windows, `C:\Users\<them>\repos\kc-employee-ownership` is fine. On a Mac,
`~/repos/kc-employee-ownership`.

Clone `https://github.com/Anthony-Ross-UMKC/kc-employee-ownership` there. It is a public
project, so this works whether or not Anthony has added them yet.

## Step 5 — Set their identity and working area

Ask for their school email address. Then, in the cloned folder:

- Set the local Git identity to their full name and that email, for this project only. Do not
  change any global setting on their machine.
- Check out the branch matching their first name, lowercase: `camron`, `kirby`, `mandy`, or
  `anthony`. Never leave them on `main`.

Do not explain what a branch is. If they ask, say it is their own copy of the project that
nobody else can disturb.

## Step 6 — Tell them where things stand

Say, in plain language:

- The project is on their computer and they are ready to work.
- The folder it is in, and that they open Claude Code there each time.
- If Anthony has not added them yet, their work saves locally and will sync as soon as he
  does. Nothing is lost in the meantime.
- The first time their work syncs, a browser window will ask them to sign in to GitHub. Use
  the account from Step 2.

Then read `ONBOARDING.md` in the project folder and give them a short summary of it in your
own words — what the project is, how the team stays out of each other's way, and the two
content rules. Do not paste the file at them.

Finally, read `TASKS.md`.

- **If it has unassigned items,** tell them they can just say what they want to work on, and
  offer one or two real examples from the list.
- **If it is empty,** say so plainly — the team has not decided what the site is made of yet,
  and that is what the Wednesday meeting is for. Tell them they are not behind, and that if
  they already have an idea of something worth doing, say it and you will add it to the list
  under their name.

Do not invent tasks to give them.

## After setup

From here on, follow `CLAUDE.md` in the project folder. It governs everything else.
