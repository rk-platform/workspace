# Changelog

What changed in each release of RK Workspace, the desktop app for
[RK](https://github.com/rk-platform/core).

## 0.2.0 (2026-10-11)

- Plugins: install from any marketplace, repository or JSON in Settings → Plugins, including plugins written for the open Agent Plugins standard. Sign in with browser, code or QR code, with more than one account.
- Marketplace: curated list of recommended plugins plus rk collection plugins.
- New plugins: collect from Reddit and Telegram, each with its own icon in the left pane and an entry in the palette.
- Graph view: the whole project as a map of documents and their links.
- The chat runs commands for you, asking their questions as cards beside the conversation.
- Long runs survive: case phases keep running when you close the window, and continue where they were after a restart or crash.
- See model cost per project and per running job, in estimated dollars.
- Images and PDFs open in a tab, and the Logs tab shows rk's whole log live.
- Faster Claude calls with warm processes, and Codex on OpenAI's newest models with login from Settings.
- Editions: the window title names yours, and commands from a higher edition are dimmed.
- Bug fixes and improvements.
- A plugin's page in Settings lists under Not used what rk left out of it: a `plugin.json` field the Agent Plugins specification does not define, an `mcp.json` it refuses, each server it skips, a key or install value of rk's it cannot use, and a `.mcp.json` it does not read. Such a plugin is marked in the Plugins list.
- The window keeps the 50 most recent finished runs whose tab is closed, and lets go of older ones and of those from a project you switch away from, so a long session no longer grows without end.
- A phase that carries on as a background job says so in its tab, with the job's number, and that closing the tab does not stop it.
- The model select in Settings shows a model's whole name, including the effort it runs at.
- The workspace waits for its project before reading the file tree, so a window opened on no project no longer shows a tree error.
- A collection or research run that carries on in the background no longer shows as failed when it starts.
- A plugin that signs in with a QR code, such as Telegram, shows a code you can scan, and Cancel stops a plugin's sign-in instead of leaving it running.
- Closing the Terminal tab ends that project's shell instead of leaving it running in the background, and asks first if a command is still running in it.
- A command or chat cut off by rk stopping or restarting ends in its tab rather than running forever, a file that will not open no longer shows rk as unreachable, and job statuses show in colour.
- Images and PDFs up to 6 MB open in a tab instead of showing only their size.
- A plugin installed or uninstalled in Settings shows in the palette and the left pane, or leaves them, without restarting the workspace, and switching projects shows that project's plugins.
- The Logs tab shows rk's whole log as it is written, background work included, starting with what was logged before you opened it.
- The Telegram plugin installs from Settings → Plugins; its research accounts sign in with a QR code from the Telegram app, and a case can collect Telegram messages with their media.
- A graph view draws the whole project as a map of documents and the links between them, with a filter per kind of document and a count of what nothing links to.
- A run's folder and a case's folder can be deleted from the tree, to the trash. The built-in folders still cannot.
- A plugin's MCP server can be a collection tool: its steps show which plugin they come from, and Settings has a Capture kept pages switch for screenshots of the pages a step keeps. The web-archive setting is gone.
- The Status tab shows what the open project has cost since you opened it, per model, in tokens and estimated dollars, and a running job shows what it has spent so far.
- A command the chat starts asks its questions as cards beside the conversation, each naming the job and opening the file it is about, while the chat stays yours to type in; the chat tells you when the job is done.
- A case phase or web research cut off by a restart or a crash continues from where it was, and a Direction cut off by a closed window continues next time, asking the waiting question again.
- Case phases read your whole case file and its status page, an Analysis now makes the score changes it proposes, and a case report no longer repeats sections under its last question.
- The chat offers skills from installed plugins and your own skill folders, and follows your AGENTS.md.
- Settings → Plugins installs plugins and MCP servers from marketplaces, a repository or JSON; rk's own plugins are under Settings → Collection plugins.
- Plugins written to the open Agent Plugins standard (agent-plugins.org) install in Settings → Plugins and run like any other.
- Plugins whose MCP server needs a sign-in, such as Gmail, have a Sign in button in Settings → Plugins, with more than one account, and bring you back to the app afterwards.
- A plugin whose MCP server signs in with its own command, such as Outlook, has a Sign in button that shows the page to open and the code to enter.
- The plugins in OpenAI's Codex marketplace (openai/plugins) can be installed; before, most were listed as not installable.
- Search results show as a list you can click, and a page a search collected can be taken into the knowledge base with a right-click.
- A web search now gives you a ranked list of the pages that answer your question, each with a line on what it says, and ingests nothing until you say so.
- Settings → Models offers OpenAI's newest Codex models: gpt-6-luna, gpt-6.1-sol and, for Large, gpt-6-astra.
- The window title names your edition, and commands from a higher edition are shown dimmed in the palette and the ribbon.
- Ask the chat to run a command and it does: questions the command asks show up in the conversation.
- Long case phases keep running when you close the window, and a second start of a running phase follows it instead of starting another.
- Settings → Models has two new fields for how many Claude processes rk keeps ready, and for how long: Claude warm processes and Claude warm-up timeout.
- You can log in to Codex from Settings, from Doctor and from the command palette, without the terminal.
- Hidden files and lock files are left out of the file tree. Show hidden files, under Workspace in Settings, shows them.

## 0.1.51 (2026-10-04)

- The rk version in the status bar follows rk when it restarts or updates, without reopening RK Workspace.

## 0.1.50 (2026-10-03)

- Bugfixes for sync and update

## 0.1.49 (2026-10-03)

- Projects can sync to a git host, turned on and off per project in Settings → Sync, which also shows the remote, the last sync and any error; a copy can be fetched onto another machine with Get project from remote, and the status bar shows how the sync stands.
- The workspace has tabs and split panes, and the tree can create, rename, move, duplicate and delete your notes, with links updated and deleted files kept in a trash you can restore from. Chat, Terminal and Logs open as tabs, every command runs in its own tab, and a finished job tells you. Cmd-O finds a file, and you can bookmark files and save layouts.
- Every text file in a project can be viewed and edited, with highlighting for its language.
- Every document can be tagged, including the ones rk writes.
- The workspace now shows what links to the open note and what it links to, with the fetch status of each web address, its outline and tags, a preview when you hover a link, and an editor for its properties.
- Tables over your notes open as editable tables, and you can make one anywhere with the New table button, blank or from a description.
- The status bar shows when rk or the app has an update, with an Update button for each.
- Notes edit in one live view that reads as rendered, with bold and italic on Cmd-B and Cmd-I and a formatting menu on right-click, find and replace, quick notes (Shift-Cmd-N), files dropped in from Finder, and a menu on web links to copy them or fetch them into the KB.
- You can attach a note to any file, entity, case or folder, and see the notes about the item you have selected under Notes in the Documents tab.
- The ? button opens a Help tab: a chat of its own that knows what you have open, welcomes you and answers from the help pages.
- Chat and every command show what they are doing while they work, with a ticking time, and keep the steps they took under the answer.
- The tree marks a collected page that was never ingested, and a right-click on it takes it into the knowledge base.

## 0.1.48 (2026-10-01)

- Opening a folder that is not a project now asks whether to make it one.
- A document the AI is writing in, such as case.md during direction, now updates on screen as it changes.

## 0.1.47 (2026-09-30)

This is the pre-alpha-1 release.
- A project's collection runs sit together under `runs/` in the tree.
- Waive a blocker from the command palette.
- Plugin support for collection plugins.
- Doctor updated.
- Improvements and bugfixes.

## 0.1.46 (2026-09-27)

- Improvements and bugfixes

## 0.1.45 (2026-09-27)

- Pre-alpha release, for Apple Silicon Macs.
