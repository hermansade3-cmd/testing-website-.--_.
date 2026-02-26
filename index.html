<!DOCTYPE html>
<html lang="sw">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SadeGpt</title>
  <link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --bg: #0a0c10;
      --surface: #111318;
      --surface2: #1a1d24;
      --border: #2a2d36;
      --accent: #00e5b0;
      --accent2: #00b8ff;
      --text: #e8ecf4;
      --muted: #6b7280;
      --user-bg: #1e2a3a;
      --ai-bg: #0f1a14;
    }

    body {
      font-family: 'Sora', sans-serif;
      background: var(--bg);
      color: var(--text);
      height: 100vh;
      display: flex;
      flex-direction: column;
      overflow: hidden;
    }

    /* Animated background */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background: 
        radial-gradient(ellipse 60% 40% at 10% 20%, rgba(0,229,176,0.06) 0%, transparent 60%),
        radial-gradient(ellipse 50% 50% at 90% 80%, rgba(0,184,255,0.05) 0%, transparent 60%);
      pointer-events: none;
      z-index: 0;
    }

    /* Header */
    header {
      position: relative;
      z-index: 10;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 16px 28px;
      border-bottom: 1px solid var(--border);
      background: rgba(10,12,16,0.85);
      backdrop-filter: blur(16px);
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .logo-icon {
      width: 36px; height: 36px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      border-radius: 10px;
      display: flex; align-items: center; justify-content: center;
      font-weight: 700; font-size: 16px; color: #000;
      box-shadow: 0 0 20px rgba(0,229,176,0.3);
    }

    .logo-text {
      font-size: 22px;
      font-weight: 700;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      letter-spacing: -0.5px;
    }

    .badge {
      font-size: 11px;
      font-family: 'JetBrains Mono', monospace;
      color: var(--accent);
      border: 1px solid rgba(0,229,176,0.3);
      padding: 3px 10px;
      border-radius: 20px;
      background: rgba(0,229,176,0.05);
    }

    /* Chat area */
    #chat {
      flex: 1;
      overflow-y: auto;
      padding: 24px 16px;
      display: flex;
      flex-direction: column;
      gap: 20px;
      position: relative;
      z-index: 1;
    }

    #chat::-webkit-scrollbar { width: 4px; }
    #chat::-webkit-scrollbar-track { background: transparent; }
    #chat::-webkit-scrollbar-thumb { background: var(--border); border-radius: 4px; }

    /* Welcome screen */
    .welcome {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      flex: 1;
      gap: 16px;
      padding: 40px 20px;
      text-align: center;
      animation: fadeUp 0.6s ease both;
    }

    .welcome-icon {
      width: 72px; height: 72px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      border-radius: 20px;
      display: flex; align-items: center; justify-content: center;
      font-size: 32px;
      box-shadow: 0 0 40px rgba(0,229,176,0.25), 0 8px 32px rgba(0,0,0,0.4);
      animation: pulse 3s ease-in-out infinite;
    }

    @keyframes pulse {
      0%, 100% { box-shadow: 0 0 40px rgba(0,229,176,0.25), 0 8px 32px rgba(0,0,0,0.4); }
      50% { box-shadow: 0 0 60px rgba(0,229,176,0.4), 0 8px 32px rgba(0,0,0,0.4); }
    }

    .welcome h1 { font-size: 28px; font-weight: 700; letter-spacing: -0.5px; }
    .welcome p { color: var(--muted); font-size: 15px; max-width: 360px; line-height: 1.6; }

    .suggestions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
      margin-top: 8px;
    }

    .suggestion-btn {
      background: var(--surface);
      border: 1px solid var(--border);
      color: var(--text);
      padding: 10px 16px;
      border-radius: 12px;
      font-size: 13px;
      font-family: 'Sora', sans-serif;
      cursor: pointer;
      transition: all 0.2s;
    }

    .suggestion-btn:hover {
      border-color: var(--accent);
      color: var(--accent);
      background: rgba(0,229,176,0.05);
      transform: translateY(-1px);
    }

    /* Messages */
    .message {
      display: flex;
      gap: 12px;
      max-width: 760px;
      width: 100%;
      margin: 0 auto;
      animation: fadeUp 0.3s ease both;
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(12px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .message.user { flex-direction: row-reverse; }

    .avatar {
      width: 36px; height: 36px;
      border-radius: 10px;
      display: flex; align-items: center; justify-content: center;
      font-size: 15px;
      flex-shrink: 0;
      font-weight: 600;
    }

    .user .avatar {
      background: linear-gradient(135deg, #2a4a8a, #1a3a6a);
      color: var(--accent2);
      border: 1px solid rgba(0,184,255,0.2);
    }

    .ai .avatar {
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      color: #000;
    }

    .bubble {
      padding: 14px 18px;
      border-radius: 16px;
      font-size: 14.5px;
      line-height: 1.7;
      max-width: calc(100% - 56px);
    }

    .user .bubble {
      background: var(--user-bg);
      border: 1px solid rgba(0,184,255,0.15);
      border-top-right-radius: 4px;
      color: var(--text);
    }

    .ai .bubble {
      background: var(--ai-bg);
      border: 1px solid rgba(0,229,176,0.12);
      border-top-left-radius: 4px;
    }

    /* Typing indicator */
    .typing-dots {
      display: flex;
      gap: 5px;
      align-items: center;
      padding: 6px 0;
    }

    .typing-dots span {
      width: 7px; height: 7px;
      background: var(--accent);
      border-radius: 50%;
      animation: dot-bounce 1.2s ease-in-out infinite;
    }

    .typing-dots span:nth-child(2) { animation-delay: 0.2s; }
    .typing-dots span:nth-child(3) { animation-delay: 0.4s; }

    @keyframes dot-bounce {
      0%, 80%, 100% { transform: scale(0.7); opacity: 0.5; }
      40% { transform: scale(1); opacity: 1; }
    }

    /* Input area */
    .input-area {
      position: relative;
      z-index: 10;
      padding: 16px 20px 20px;
      border-top: 1px solid var(--border);
      background: rgba(10,12,16,0.9);
      backdrop-filter: blur(16px);
    }

    .input-wrapper {
      max-width: 760px;
      margin: 0 auto;
      display: flex;
      gap: 10px;
      align-items: flex-end;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 10px 12px 10px 16px;
      transition: border-color 0.2s, box-shadow 0.2s;
    }

    .input-wrapper:focus-within {
      border-color: rgba(0,229,176,0.4);
      box-shadow: 0 0 0 3px rgba(0,229,176,0.06);
    }

    #user-input {
      flex: 1;
      background: none;
      border: none;
      outline: none;
      color: var(--text);
      font-family: 'Sora', sans-serif;
      font-size: 14.5px;
      resize: none;
      max-height: 160px;
      line-height: 1.6;
    }

    #user-input::placeholder { color: var(--muted); }

    #send-btn {
      width: 38px; height: 38px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      border: none;
      border-radius: 10px;
      cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      flex-shrink: 0;
      transition: transform 0.15s, opacity 0.15s;
      color: #000;
    }

    #send-btn:hover:not(:disabled) { transform: scale(1.05); }
    #send-btn:active:not(:disabled) { transform: scale(0.96); }
    #send-btn:disabled { opacity: 0.4; cursor: not-allowed; }

    .input-hint {
      text-align: center;
      font-size: 11px;
      color: var(--muted);
      margin-top: 8px;
      font-family: 'JetBrains Mono', monospace;
    }

    /* Code blocks in responses */
    .bubble pre {
      background: #0a0c0f;
      border: 1px solid var(--border);
      border-radius: 8px;
      padding: 12px;
      overflow-x: auto;
      margin: 8px 0;
      font-family: 'JetBrains Mono', monospace;
      font-size: 13px;
    }

    .bubble strong { color: var(--accent); }
  </style>
</head>
<body>

<header>
  <div class="logo">
    <div class="logo-icon">S</div>
    <span class="logo-text">SadeGpt</span>
  </div>
  <div class="badge">v1.0 · AI Assistant</div>
</header>

<div id="chat">
  <div class="welcome" id="welcome">
    <div class="welcome-icon">🤖</div>
    <h1>Karibu SadeGpt</h1>
    <p>Niulize swali lolote — nitakusaidia kupata jibu sahihi na la haraka.</p>
    <div class="suggestions">
      <button class="suggestion-btn" onclick="askSuggestion(this)">🌍 Mji mkuu wa Ufaransa ni nini?</button>
      <button class="suggestion-btn" onclick="askSuggestion(this)">📚 Nifundishe kuhusu AI</button>
      <button class="suggestion-btn" onclick="askSuggestion(this)">🔢 2 + 2 ni ngapi?</button>
      <button class="suggestion-btn" onclick="askSuggestion(this)">💡 Nisaidie kuandika barua pepe</button>
    </div>
  </div>
</div>

<div class="input-area">
  <div class="input-wrapper">
    <textarea 
      id="user-input" 
      placeholder="Andika swali lako hapa..." 
      rows="1"
      onkeydown="handleKey(event)"
      oninput="autoResize(this)"
    ></textarea>
    <button id="send-btn" onclick="sendMessage()" title="Tuma">
      <svg width="18" height="18" fill="none" viewBox="0 0 24 24">
        <path d="M5 12h14M12 5l7 7-7 7" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </button>
  </div>
  <div class="input-hint">Enter kutuma · Shift+Enter mstari mpya</div>
</div>

<script>
  const chatEl = document.getElementById('chat');
  const inputEl = document.getElementById('user-input');
  const sendBtn = document.getElementById('send-btn');
  let isLoading = false;
  const history = [];

  function autoResize(el) {
    el.style.height = 'auto';
    el.style.height = Math.min(el.scrollHeight, 160) + 'px';
  }

  function handleKey(e) {
    if (e.key === 'Enter' && !e.shiftKey) {
      e.preventDefault();
      sendMessage();
    }
  }

  function askSuggestion(btn) {
    inputEl.value = btn.textContent.replace(/^[^\w\s]+\s/, '').trim();
    sendMessage();
  }

  function removeWelcome() {
    const w = document.getElementById('welcome');
    if (w) w.remove();
  }

  function addMessage(role, text) {
    removeWelcome();
    const div = document.createElement('div');
    div.className = `message ${role}`;
    const avatarText = role === 'user' ? 'W' : 'S';
    div.innerHTML = `
      <div class="avatar">${avatarText}</div>
      <div class="bubble">${formatText(text)}</div>
    `;
    chatEl.appendChild(div);
    chatEl.scrollTop = chatEl.scrollHeight;
    return div;
  }

  function addTypingIndicator() {
    removeWelcome();
    const div = document.createElement('div');
    div.className = 'message ai';
    div.id = 'typing';
    div.innerHTML = `
      <div class="avatar">S</div>
      <div class="bubble">
        <div class="typing-dots"><span></span><span></span><span></span></div>
      </div>
    `;
    chatEl.appendChild(div);
    chatEl.scrollTop = chatEl.scrollHeight;
  }

  function removeTypingIndicator() {
    const t = document.getElementById('typing');
    if (t) t.remove();
  }

  function formatText(text) {
    return text
      .replace(/```([\s\S]*?)```/g, '<pre><code>$1</code></pre>')
      .replace(/`([^`]+)`/g, '<code style="font-family:JetBrains Mono,monospace;background:#1a1d24;padding:2px 6px;border-radius:4px;font-size:13px">$1</code>')
      .replace(/\*\*(.*?)\*\*/g, '<strong>$1</strong>')
      .replace(/\n/g, '<br>');
  }

  async function sendMessage() {
    const text = inputEl.value.trim();
    if (!text || isLoading) return;

    inputEl.value = '';
    inputEl.style.height = 'auto';
    isLoading = true;
    sendBtn.disabled = true;

    addMessage('user', text);
    history.push({ role: 'user', content: text });

    addTypingIndicator();

    try {
      const response = await fetch('https://api.anthropic.com/v1/messages', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({
          model: 'claude-sonnet-4-20250514',
          max_tokens: 1000,
          system: 'Wewe ni SadeGpt, msaidizi wa akili bandia wa Kiswahili. Jibu maswali kwa Kiswahili fasaha, kwa ufupi na usahihi. Kama swali liko kwa Kiingereza au lugha nyingine, jibu kwa lugha ile ile.',
          messages: history
        })
      });

      const data = await response.json();
      const reply = data.content?.[0]?.text || 'Samahani, kuna hitilafu. Jaribu tena.';

      removeTypingIndicator();
      history.push({ role: 'assistant', content: reply });
      addMessage('ai', reply);

    } catch (err) {
      removeTypingIndicator();
      addMessage('ai', '⚠️ Kuna tatizo la mtandao. Tafadhali angalia muunganisho wako na ujaribu tena.');
    }

    isLoading = false;
    sendBtn.disabled = false;
    inputEl.focus();
  }
</script>
</body>
</html>
