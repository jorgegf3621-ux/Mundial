# World Cup 2026 Quiz - Amalga Group

Multiplayer football trivia game for a Team Wide Call.

## Structure

```text
mundial-quiz/
├── index.html      <- Main app
├── questions.js    <- 200+ question bank in easy / medium / hard batches
├── vercel.json     <- Vercel config
├── .gitignore
└── README.md
```

## How to use

### Host
1. Open `index.html` in the browser.
2. Enter a Room ID such as `amalga2026`.
3. Click `Host View`.
4. Share the generated team links with players.

### Player
1. Open the shared link or enter the Room ID manually.
2. Pick your country.
3. Enter your name and player number.
4. Click `Player View`.

## Tournament format

- 8 teams: Mexico, Brazil, Spain, Argentina, France, Germany, Portugal, United States
- Knockout bracket: Quarterfinals -> Semifinals -> Grand Final
- First team to 3 goals wins each match
- 200+ possible questions with multiple choice answers
- Difficulty rotation: easy -> medium -> hard -> repeat
- Music, confetti, and sound effects included

## Deploy on Vercel

1. Push this folder to a GitHub repository.
2. Import the repo on `vercel.com`.
3. Use `Other` as the framework preset.
4. Leave build and output settings empty.
5. Deploy.

## Multiplayer note

The game syncs through `localStorage` and `BroadcastChannel`.
It works across tabs in the same browser.
For true multi-device realtime play, a backend such as Supabase Realtime would be needed.
