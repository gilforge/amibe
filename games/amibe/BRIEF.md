# Amibe

Aider une créature simple à se nourrir et se reproduire.

---

## The JumPHP playground

This project was made on the JumPHP playground: the game's page is https://jumphp.net/amibe
(category: Démos et expériences).

- The game is `games/amibe/`. Read `AGENTS.md` (the JumPHP contract) first; replace the skeleton with the game
  described above; follow the definition of done (tests, screenshots you look at, browser build).
- **Publishing**: every push to `main` is online within a minute (GitHub webhook). The MCP tool
  `sync_project` (server `jumphp`) publishes at once and returns the errors: a commit with a PHP syntax error
  is not published (the previous version stays online).
- The playground loads the game file by file with its shared engine: Composer packages other than
  `jumphp/engine` are not available there.
- **The game's home page**: make `games/amibe/site/` (AGENTS.md section 13: themed with the game's own graphics,
  SEO, a link to `play/`); it is the game's page on the playground. Also `games/amibe/assets/thumbnail.png`.
- When the game is done: MCP `update_project` with `listed: true` shows it in the playground's directory.