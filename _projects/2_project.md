---
layout: page
title: Compai
description: A RAG companion chatbot on Telegram that adapts to a chosen speaker's style.
img: assets/img/projects/compai.jpg
importance: 2
---

<style>
  html:not([data-theme="dark"]) {
    --global-bg-color: #fbf1ee; --global-card-bg-color: #ffffff; --global-text-color: #3d2a33; --global-text-color-light: #8a6f78;
    --global-theme-color: #d9576f; --global-hover-color: #d9576f; --global-divider-color: rgba(61, 42, 51, 0.12);
    --global-footer-bg-color: #3d2a33; --global-footer-text-color: #fbf1ee; --global-footer-link-color: #ffffff;
  }
  .cp { --cp-card: #ffffff; --cp-ink: #3d2a33; --cp-rose: #d9576f; --cp-apricot: #f2a65a; --cp-blush: #f6dcd8; }
  .cp-link { display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.5rem 1.1rem; border: 1.5px solid var(--global-text-color); border-radius: 999px; color: var(--global-text-color); font-size: 1rem; text-decoration: none; }
  .cp-link:hover { border-color: var(--global-theme-color); color: var(--global-theme-color); text-decoration: none; }
  .cp-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; margin: 1rem 0 2rem; }
  .cp-tag { padding: 0.15rem 0.7rem; border-radius: 999px; font-size: 0.85rem; font-weight: 600; }
  .cp-tag.rose { background: var(--cp-rose); color: #fff; }
  .cp-tag.apricot { background: var(--cp-apricot); color: var(--cp-ink); }
  .cp-video { margin-bottom: 2.5rem; }
  .cp-video iframe { display: block; width: 100%; aspect-ratio: 16 / 9; height: auto; border: 0; border-radius: 8px; box-shadow: 0 2px 10px rgba(61, 42, 51, 0.18); }
  .cp-meta { display: flex; flex-wrap: wrap; gap: 2.5rem; margin: 0.5rem 0 2rem; }
  .cp-meta > div { display: flex; flex-direction: column; gap: 0.15rem; }
  .cp-meta .k, .cp-stack .k { font-size: 0.75rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.1em; color: var(--global-text-color-light); }
  .cp-meta .v { font-size: 1rem; font-weight: 600; color: var(--global-text-color); }
  .cp h2 { font-size: 0.8rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.14em; color: var(--global-theme-color); margin: 2.5rem 0 1rem; }
  .cp-features { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1rem; }
  .cp, .cp p, .cp li { font-size: 1rem; line-height: 1.7; }
  .cp-feature { background: transparent; color: var(--cp-ink); border: 1.5px solid var(--global-text-color); border-radius: 12px; padding: 1rem 1.2rem; }
  .cp-feature h3 { font-size: 1rem; font-weight: 600; margin: 0 0 0.3rem; color: var(--cp-ink); }
  .cp-feature h3 i { margin-right: 0.35rem; color: var(--cp-rose); }
  .cp-feature p { margin: 0; }
  .cp-steps { list-style: none; counter-reset: step; padding: 0; margin: 0; }
  .cp-steps li { counter-increment: step; position: relative; padding: 0 0 1.2rem 3rem; }
  .cp-steps li::before { content: counter(step); position: absolute; left: 0; top: -0.1rem; width: 2rem; height: 2rem; border-radius: 50%; background: var(--cp-rose); color: #fff; font-weight: 700; display: flex; align-items: center; justify-content: center; }
  .cp-steps li:not(:last-child)::after { content: ""; position: absolute; left: calc(1rem - 1px); top: 2rem; bottom: 0.1rem; width: 2px; background: var(--cp-blush); }
  .cp-steps strong { color: var(--cp-ink); }
  .cp-stack { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; }
  .cp-stack > div { display: flex; flex-direction: column; align-items: flex-start; gap: 0.4rem; background: transparent; border: 1.5px solid var(--global-text-color); border-radius: 12px; padding: 0.9rem 1.1rem; }
  .cp-stack .tags { display: flex; flex-wrap: wrap; gap: 0.3rem; }
  .cp-future { padding-left: 1.2rem; margin: 0; }
  .cp-future li { margin-bottom: 0.4rem; }
  @media (max-width: 700px) { .cp-features { grid-template-columns: 1fr; } .cp-stack { grid-template-columns: repeat(2, 1fr); } }
</style>

<div class="cp">
  <a class="cp-link" href="https://github.com/FLYIH/Compai" target="_blank" rel="noopener"><i class="fa-brands fa-github"></i> FLYIH/Compai</a>
  <div class="cp-tags">
    <span class="cp-tag rose">Chatbot</span>
    <span class="cp-tag apricot">RAG</span>
  </div>
  <div class="cp-video">
    <iframe src="https://www.youtube-nocookie.com/embed/54qxNNAtHT0?rel=0" title="Compai demo" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy"></iframe>
  </div>
  <div class="cp-meta">
    <div><span class="k">Timeline</span><span class="v">2025.02 – 2025.03</span></div>
    <div><span class="k">Team</span><span class="v">4 members</span></div>
    <div><span class="k">Role</span><span class="v">Architect &amp; Lead Developer</span></div>
    <div><span class="k">Program</span><span class="v">CS Equity AI Bootcamp</span></div>
  </div>
  <h2>Overview</h2>
  <p>
    <strong>Compai</strong> is a companion chatbot that lets users chat with a virtual version of someone they wish to speak to,
    reproducing that person's speaking style in any scenario. It is designed as a safe and controlled emotional outlet.
    Users upload an exported Telegram chat history; Compai learns the speaker's style from it and answers through a Telegram bot,
    using retrieval-augmented generation (RAG) over past conversations with the Gemini API and ChromaDB.
  </p>
  <h2>Key Features</h2>
  <div class="cp-features">
    <div class="cp-feature">
      <h3><i class="fa-solid fa-clock-rotate-left"></i> Short-term Memory</h3>
      <p>Keeps the last five messages in a double-ended queue so replies stay on topic.</p>
    </div>
    <div class="cp-feature">
      <h3><i class="fa-solid fa-brain"></i> Long-term Memory</h3>
      <p>Extracts details such as age, preferences, and dislikes from history into key-value records for more relevant responses.</p>
    </div>
    <div class="cp-feature">
      <h3><i class="fa-solid fa-masks-theater"></i> Speaker Style Adaptation</h3>
      <p>Analyzes writing style, tone, and emoji usage so responses sound like the designated speaker.</p>
    </div>
    <div class="cp-feature">
      <h3><i class="fa-brands fa-telegram"></i> Telegram Integration</h3>
      <p>Accepts an uploaded chat history and automatically recognizes both users' IDs, then chats in real time.</p>
    </div>
  </div>
  <h2>How It Works</h2>
  <ol class="cp-steps">
    <li><strong>Ingest.</strong> The exported Telegram JSON is loaded in chunks with orjson, embedded, and stored in a ChromaDB collection.</li>
    <li><strong>Learn the style.</strong> The speaker's communication style is analyzed from the conversation history.</li>
    <li><strong>Retrieve.</strong> For each query, RAG searches ChromaDB for similar past conversations and combines them with the stored key-value facts and the last five messages.</li>
    <li><strong>Generate.</strong> Gemini (gemini-1.5-flash) produces a reply from this combined context and the speaker's style, so it feels natural and personalized.</li>
  </ol>
  <h2>My Role</h2>
  <div class="cp-features">
    <div class="cp-feature">
      <h3><i class="fa-solid fa-sitemap"></i> System Architecture</h3>
      <p>Designed the overall pipeline: how chat history is ingested, how short- and long-term memory and RAG retrieval are combined, and how responses are generated.</p>
    </div>
    <div class="cp-feature">
      <h3><i class="fa-solid fa-code"></i> Lead Developer</h3>
      <p>Wrote most of the codebase, implementing the memory, retrieval, and generation modules.</p>
    </div>
  </div>
  <h2>Performance Optimization</h2>
  <p><strong>Embedding acceleration:</strong> conversation data is embedded in batches instead of message by message, which reduces the number of API calls.</p>
  <h2>Results</h2>
  <p>
    Compai adapts accurately to the designated speaker's style. The style can also be changed easily through the prompt for any desired tone,
    for example a "warm &amp; sweet" chat environment.
  </p>
  <h2>Future Work</h2>
  <ul class="cp-future">
    <li>More human-like responses</li>
    <li>Voice message support</li>
    <li>Multi-user support</li>
  </ul>
  <h2>Tech Stack</h2>
  <div class="cp-stack">
    <div><span class="k">Language</span><div class="tags"><span class="cp-tag rose">Python</span></div></div>
    <div><span class="k">LLM</span><div class="tags"><span class="cp-tag apricot">Gemini 1.5 Flash</span></div></div>
    <div><span class="k">Retrieval</span><div class="tags"><span class="cp-tag rose">ChromaDB</span><span class="cp-tag apricot">PaLM Embeddings</span></div></div>
    <div><span class="k">Interface</span><div class="tags"><span class="cp-tag rose">Telegram Bot</span></div></div>
  </div>
</div>
