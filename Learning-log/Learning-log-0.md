Learning Log

Week 0 — 2026-09-07 (Lab Setup)

Built:
- I set up my Mac Mini M4 pro server via:
    - Local SSH
    - Meshnet SSH

- 

Broke:
    - git clone → "Repository not found": wrong username in the URL.

    - ollama run gemma 4 downloaded a 2024 model. (Be specific about the model you want to use)

Can explain:
    - A repo URL contains the account name that owns it, which may not be the name you expected.

    - ssh -T git@github.com saying "no shell access" is success. GitHub authenticates you and hangs up because there's nothing to log into.

    - Git's user.name is just a label on commits; user.email is what links commits to your GitHub account.

    The Ollama menu-bar app supervises its server: kill the server and the app restarts it. You have to quit the app (killall Ollama, capital O; pkill is case-sensitive).

    - An SSH session is its own terminal. Nothing you do there shows on the remote machine's screen, and foreground commands (like a pull) die with the session; background ones don't.

Can't explain yet:
    - Why my local

Hours: 8 hours