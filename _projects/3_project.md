---
layout: page
title: Kahoot
description: A real-time multiplayer quiz game over TCP sockets, with a C server and an SFML client.
img: assets/img/projects/kahoot.jpg
importance: 3
---

<style>
  html:not([data-theme="dark"]) {
    --global-bg-color: #fbf3c4; --global-card-bg-color: #fdf8dc; --global-text-color: #2b2a24; --global-text-color-light: #786f4e;
    --global-theme-color: #23897a; --global-hover-color: #23897a; --global-divider-color: rgba(43, 42, 36, 0.15);
    --global-footer-bg-color: #23897a; --global-footer-text-color: #fbf3c4; --global-footer-link-color: #ffffff;
  }
  .kh { --kh-teal: #2a9988; --kh-yellow: #f5c518; --kh-sand: #c9bb8e; --kh-ink: #2b2a24; }
  .kh, .kh p, .kh li { font-size: 1rem; line-height: 1.7; }
  .kh-link { display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.5rem 1.1rem; border: 1.5px solid var(--global-text-color); border-radius: 999px; color: var(--global-text-color); font-size: 1rem; text-decoration: none; }
  .kh-link:hover { border-color: var(--global-theme-color); color: var(--global-theme-color); text-decoration: none; }
  .kh-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; margin: 1rem 0 2rem; }
  .kh-tag { padding: 0.15rem 0.7rem; border-radius: 999px; font-size: 0.85rem; font-weight: 600; }
  .kh-tag.teal { background: var(--kh-teal); color: #fff; }
  .kh-tag.yellow { background: var(--kh-yellow); color: var(--kh-ink); }
  .kh-video { margin-bottom: 2.5rem; }
  .kh-video iframe { display: block; width: 100%; aspect-ratio: 16 / 9; height: auto; border: 0; border-radius: 8px; box-shadow: 0 2px 10px rgba(43, 42, 36, 0.18); }
  .kh-meta { display: flex; flex-wrap: wrap; gap: 2.5rem; margin: 0.5rem 0 2rem; }
  .kh-meta > div { display: flex; flex-direction: column; gap: 0.15rem; }
  .kh-meta .k, .kh-stack .k { font-size: 0.75rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.1em; color: var(--global-text-color-light); }
  .kh-meta .v { font-size: 1rem; font-weight: 600; color: var(--global-text-color); }
  .kh h2 { font-size: 0.8rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.14em; color: var(--global-theme-color); margin: 2.5rem 0 1rem; }
  .kh-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1rem; }
  .kh-card { border: 1.5px solid var(--global-text-color); border-radius: 12px; padding: 1rem 1.2rem; color: var(--kh-ink); }
  .kh-card h3 { font-size: 1rem; font-weight: 600; margin: 0 0 0.3rem; color: var(--kh-ink); }
  .kh-card h3 i { margin-right: 0.35rem; color: var(--kh-teal); }
  .kh-card p { margin: 0; }
  .kh-card ul { margin: 0.3rem 0 0; padding-left: 1.1rem; }
  .kh-card code, .kh p code { font-size: 0.9em; background: rgba(42, 153, 136, 0.12); color: var(--kh-ink); padding: 0.05rem 0.35rem; border-radius: 4px; }
  .kh-flow { display: flex; flex-wrap: wrap; align-items: center; gap: 0.5rem; margin: 0.5rem 0 0; }
  .kh-flow span { padding: 0.35rem 0.9rem; border-radius: 6px; background: var(--kh-teal); color: #fff; font-weight: 600; font-size: 0.9rem; }
  .kh-flow i { color: var(--global-text-color-light); font-size: 0.8rem; }
  .kh-challenge { padding: 1rem 0; border-bottom: 1px solid var(--global-divider-color); }
  .kh-challenge:last-child { border-bottom: none; }
  .kh-challenge .q { font-weight: 600; margin-bottom: 0.2rem; }
  .kh-challenge .a { color: var(--global-text-color); }
  .kh-challenge .a::before { content: "→ "; color: var(--kh-teal); font-weight: 700; }
  .kh-stack { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; }
  .kh-stack > div { display: flex; flex-direction: column; align-items: flex-start; gap: 0.4rem; background: rgba(255, 255, 255, 0.6); border-radius: 12px; padding: 0.9rem 1.1rem; }
  .kh-stack .tags { display: flex; flex-wrap: wrap; gap: 0.3rem; }
  .kh-future { padding-left: 1.2rem; margin: 0; }
  @media (max-width: 700px) { .kh-grid { grid-template-columns: 1fr; } .kh-stack { grid-template-columns: repeat(2, 1fr); } }
</style>

<div class="kh">
  <a class="kh-link" href="https://github.com/FLYIH/Kahoot" target="_blank" rel="noopener"><i class="fa-brands fa-github"></i> FLYIH/Kahoot</a>
  <div class="kh-tags">
    <span class="kh-tag teal">Network Programming</span>
    <span class="kh-tag yellow">Multiplayer Game</span>
  </div>
  <div class="kh-video">
    <iframe src="https://www.youtube-nocookie.com/embed/n9zhfwTx_iU?rel=0" title="Kahoot demo" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy"></iframe>
  </div>
  <div class="kh-meta">
    <div><span class="k">Course</span><span class="v">Network Programming (Final Project)</span></div>
    <div><span class="k">Team</span><span class="v">2 members</span></div>
    <div><span class="k">Role</span><span class="v">Client &amp; GUI Developer</span></div>
  </div>
  <h2>Overview</h2>
  <p>
    A real-time multiplayer quiz game modeled on Kahoot, built on a client–server architecture over TCP sockets.
    A multithreaded C server hosts up to four game rooms of four players each (16 concurrent players), runs the rounds, and scores the answers;
    a C++ client with an SFML graphical interface lets players join a room, answer timed questions, and follow live results.
    Players can also upload their own question banks to the server.
  </p>
  <h2>Key Features</h2>
  <div class="kh-grid">
    <div class="kh-card">
      <h3><i class="fa-solid fa-users"></i> Multiplayer Rooms</h3>
      <p>A game starts once four players join a room; the server runs up to four rooms in parallel with one thread per room.</p>
    </div>
    <div class="kh-card">
      <h3><i class="fa-solid fa-stopwatch"></i> Timed Rounds</h3>
      <p>Each question has a countdown; unanswered questions score zero, and the highest total score wins.</p>
    </div>
    <div class="kh-card">
      <h3><i class="fa-solid fa-ranking-star"></i> Live Results</h3>
      <p>After every question, players see the answer distribution, their own result, and the current scoreboard.</p>
    </div>
    <div class="kh-card">
      <h3><i class="fa-solid fa-file-arrow-up"></i> Custom Question Banks</h3>
      <p>Players upload <code>.txt</code> question files, which the server validates and adds to its question pool.</p>
    </div>
  </div>
  <h2>Architecture</h2>
  <div class="kh-grid">
    <div class="kh-card">
      <h3><i class="fa-solid fa-server"></i> Server (C)</h3>
      <ul>
        <li>Spawns a <code>pthread</code> per game room</li>
        <li>Uses <code>select</code> to receive answers from all players concurrently</li>
        <li>Locks a room with a mutex while a game is running so no one joins mid-game</li>
        <li>Handles disconnects and resets the room when a game ends</li>
      </ul>
    </div>
    <div class="kh-card">
      <h3><i class="fa-solid fa-display"></i> Client (C++ / SFML)</h3>
      <p>A state machine that switches screens based on server notifications:</p>
      <div class="kh-flow">
        <span>Main Menu</span><i class="fa-solid fa-chevron-right"></i>
        <span>Waiting Room</span><i class="fa-solid fa-chevron-right"></i>
        <span>Quiz</span><i class="fa-solid fa-chevron-right"></i>
        <span>Result</span><i class="fa-solid fa-chevron-right"></i>
        <span>Scoreboard</span>
      </div>
    </div>
  </div>
  <h2>My Role</h2>
  <div class="kh-grid">
    <div class="kh-card">
      <h3><i class="fa-solid fa-gamepad"></i> Game Design</h3>
      <p>Co-designed the game flow and the client–server message protocol.</p>
    </div>
    <div class="kh-card">
      <h3><i class="fa-solid fa-code"></i> Client &amp; GUI</h3>
      <p>Wrote the entire client and drew every screen in SFML: the main menu, waiting room, quiz with countdown bar, result, and scoreboard.</p>
    </div>
  </div>
  <h2>Challenges &amp; Solutions</h2>
  <div class="kh-challenge">
    <div class="q">Keeping the GUI in sync with the server</div>
    <div class="a">Rendering and listening with <code>select</code> run in the same loop, so the UI sometimes drew before a message arrived. We introduced fixed notification strings that the client can recognize immediately to switch screens.</div>
  </div>
  <div class="kh-challenge">
    <div class="q">Missed messages when the server sends too fast</div>
    <div class="a">Added short 100–200 ms gaps between notifications and other messages so the client has time to read each one.</div>
  </div>
  <div class="kh-challenge">
    <div class="q">Byte-order mismatch between Linux and macOS</div>
    <div class="a">Used <code>htobe64</code> / <code>be64toh</code> with conditional compilation so file sizes are transferred consistently on both platforms.</div>
  </div>
  <h2>Future Work</h2>
  <ul class="kh-future">
    <li>More rooms and players per room</li>
    <li>Joining a specific room with a room code</li>
    <li>Choosing a question bank by topic or difficulty</li>
    <li>Multiple-choice and free-text question types</li>
    <li>A multithreaded client to avoid UI stalls</li>
  </ul>
  <h2>Tech Stack</h2>
  <div class="kh-stack">
    <div><span class="k">Language</span><div class="tags"><span class="kh-tag teal">C</span><span class="kh-tag teal">C++</span></div></div>
    <div><span class="k">Networking</span><div class="tags"><span class="kh-tag yellow">TCP Sockets</span><span class="kh-tag yellow">select</span></div></div>
    <div><span class="k">Concurrency</span><div class="tags"><span class="kh-tag teal">pthreads</span><span class="kh-tag teal">mutex</span></div></div>
    <div><span class="k">GUI</span><div class="tags"><span class="kh-tag yellow">SFML</span></div></div>
  </div>
</div>
