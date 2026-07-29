<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Linkup Management LLC - Email Signature Generator</title>
  <style>
    :root {
      --border:#e5e7eb; --text:#111827; --muted:#6b7280; --bg:#ffffff; --panel:#f9fafb;
    }
    * { box-sizing: border-box; }
    body { margin:0; font-family: Arial, Helvetica, sans-serif; color: var(--text); background: var(--bg); }
    .wrap { max-width: 1100px; margin: 0 auto; padding: 24px; }
    h1 { font-size: 22px; margin: 0 0 10px; }
    p { margin: 0 0 18px; color: var(--muted); line-height: 1.5; }
    .grid { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; }
    @media (max-width: 900px) { .grid { grid-template-columns: 1fr; } }

    .card { border: 1px solid var(--border); border-radius: 14px; background: var(--panel); padding: 16px; }
    .card h2 { font-size: 14px; margin: 0 0 12px; color: #111827; letter-spacing: .02em; }

    label { display:block; font-size: 12px; color: var(--muted); margin: 12px 0 6px; }
    input, textarea {
      width:100%; border:1px solid var(--border); border-radius: 10px; padding: 10px 12px;
      font-family: Arial, Helvetica, sans-serif; font-size: 14px; background:#fff; color:#111827;
      outline: none;
    }
    input:focus, textarea:focus { border-color:#9ca3af; }
    textarea {
      min-height: 220px; resize: vertical;
      font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
      font-size: 12px; line-height: 1.45;
    }

    .row { display:grid; grid-template-columns: 1fr 1fr; gap: 12px; }
    @media (max-width: 520px) { .row { grid-template-columns: 1fr; } }

    .btns { display:flex; gap:10px; flex-wrap:wrap; margin-top: 14px; }
    button {
      border: 1px solid var(--border); background:#fff; color:#111827;
      padding: 10px 12px; border-radius: 10px; cursor:pointer; font-size: 14px;
    }
    button.primary {
      background:#111827; color:#fff; border-color:#111827;
      font-weight: 700; padding: 12px 16px; box-shadow: 0 1px 2px rgba(0,0,0,.12);
      min-width: 220px;
    }
    button.primary:hover { opacity: .94; }
    button.secondary { background:#fff; color:#111827; border-color:#9ca3af; }
    button.secondary:hover { border-color:#6b7280; }
    button:active { transform: translateY(1px); }

    .previewBox { background:#fff; border:1px solid var(--border); border-radius: 12px; padding: 14px; overflow:auto; }
    .hint { font-size: 12px; color: var(--muted); margin-top: 10px; line-height: 1.45; }
    .status { font-size: 12px; color: #065f46; margin-top: 10px; display:none; }
    .status.show { display:block; }
    .danger { color:#b91c1c; }
    .footer { margin-top: 18px; text-align: center; font-size: 12px; color: var(--muted); }
  </style>
</head>
<body>
  <div class="wrap">
    <h1>Linkup Management LLC · Email Signature Generator</h1>
    <p>填写信息 → 预览 → 复制粘贴到 Gmail 的签名设置里即可。</p>

    <div class="grid">
      <div class="card">
        <h2>1) 填写信息</h2>

        <div class="row">
          <div>
            <label for="name">姓名</label>
            <input id="name" type="text" placeholder="First Name Last Name" autocomplete="name" />
          </div>
          <div>
            <label for="title">职位</label>
            <input id="title" type="text" placeholder="Title" />
          </div>
        </div>

        <div class="row">
          <div>
            <label for="phone">电话</label>
            <input id="phone" type="text" placeholder="Phone" inputmode="tel" autocomplete="tel" />
          </div>
          <div>
            <label for="email">邮箱</label>
            <input id="email" type="email" placeholder="Email" autocomplete="email" />
          </div>
        </div>

        <div>
          <label for="website">网址</label>
          <input id="website" type="text" placeholder="Website" />
        </div>

        <div>
          <label for="address">地址</label>
          <input id="address" type="text" placeholder="Address" />
        </div>

        <div class="btns">
          <button class="primary" id="copyRichBtn" type="button">Copy formatted signature</button>
          <button class="secondary" id="copyBtn" type="button">Copy HTML (backup)</button>
          <button id="resetBtn" type="button">Reset</button>
        </div>

        <div id="status" class="status">Copied ✅</div>

        <div class="hint">
          <div><strong>建议：</strong>优先使用 <b>Copy formatted signature</b>（Chrome/Edge 最稳定）。如果粘贴到 Gmail 后样式丢失，就用 <b>Copy HTML (backup)</b>，或先粘贴到 Google Docs 再复制到 Gmail。</div>
        </div>
      </div>

      <div class="card">
        <h2>2) 预览</h2>
        <div class="previewBox" id="preview" aria-label="signature preview"></div>

        <label for="output">3) HTML 输出（备份用）</label>
        <textarea id="output" spellcheck="false"></textarea>

        <div class="hint">
          <strong>Gmail 设置路径：</strong>
          <ol style="margin:8px 0 0 18px; color: var(--muted);">
            <li>Gmail 右上角 ⚙️ → <em>See all settings</em></li>
            <li>找到 <em>Signature</em> → <em>Create new</em></li>
            <li>在编辑框里粘贴你的签名 → 底部 <em>Save Changes</em></li>
          </ol>
        </div>
      </div>
    </div>

    <div class="footer">Design by Ryan Yang 2026</div>
  </div>

  <script>
    // Logo URL (direct link). Keep it as a direct i.imgur.com link for best reliability in email clients.
    const LOGO_URL = "https://i.imgur.com/RGy4egF.png"; // direct Imgur image link
    // If your logo uses a different extension, try .jpg or .jpeg
    const LOGO_WIDTH = 120;

    const el = (id) => document.getElementById(id);
    const nameEl = el('name');
    const titleEl = el('title');
    const phoneEl = el('phone');
    const emailEl = el('email');
    const websiteEl = el('website');
    const addressEl = el('address');
    const previewEl = el('preview');
    const outputEl = el('output');
    const statusEl = el('status');

    function escapeHtml(str) {
      return String(str)
        .replaceAll('&', '&amp;')
        .replaceAll('<', '&lt;')
        .replaceAll('>', '&gt;')
        .replaceAll('"', '&quot;')
        .replaceAll("'", '&#39;');
    }

    function normalizeEmail(raw) {
      return String(raw || '').trim();
    }

    function buildSignatureHTML({ name, title, phone, email, website, address }) {
      const safeName = escapeHtml((name || '').trim() || 'First Name Last Name');
      const safeTitle = escapeHtml((title || '').trim() || 'Title');
      const safePhone = escapeHtml((phone || '').trim() || 'Phone');

      const safeEmail = normalizeEmail(email);
      const mailtoEmail = safeEmail || 'email@company.com';
      const safeEmailText = safeEmail ? escapeHtml(safeEmail) : 'Email';

      const rawWebsite = String(website || '').trim();
      const websiteDisplay = rawWebsite || 'Website';
      const websiteHref = rawWebsite
        ? (/^https?:\/\//i.test(rawWebsite) ? rawWebsite : `https://${rawWebsite}`)
        : 'https://example.com';
      const safeWebsiteText = escapeHtml(websiteDisplay.replace(/^https?:\/\//i, ''));
      const safeWebsiteHref = escapeHtml(websiteHref);

      const safeAddress = escapeHtml((address || '').trim() || 'Address');

      const iconColor = '#6E86B6';
      const primaryText = '#5F6368';
      const secondaryText = '#6B7280';

      const phoneIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="${iconColor}" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6A19.79 19.79 0 0 1 2.12 4.18 2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72c.12.9.33 1.78.63 2.62a2 2 0 0 1-.45 2.11L8 9.91a16 16 0 0 0 6.09 6.09l1.46-1.29a2 2 0 0 1 2.11-.45c.84.3 1.72.51 2.62.63A2 2 0 0 1 22 16.92z"/></svg>`;
      const globeIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="${iconColor}" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><path d="M2 12h20"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>`;
      const mailIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="${iconColor}" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="5" width="18" height="14" rx="2" ry="2"/><path d="M3 7l9 6 9-6"/></svg>`;
      const pinIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="${iconColor}" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M21 10c0 7-9 13-9 13S3 17 3 10a9 9 0 1 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>`;

      return `<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
</head>
<body>
<table cellpadding="0" cellspacing="0" border="0" style="font-family: Arial, Helvetica, sans-serif; font-size: 14px; line-height: 22px; color: ${primaryText};">
  <tr>
    <td style="padding-right: 12px; vertical-align: middle; width: 132px;">
      <div style="text-align: center; width: 120px; margin: 0 auto;">
        <img src="${LOGO_URL}" alt="Linkup Management LLC" width="${LOGO_WIDTH}" style="display:block; border:0; margin: 0 auto;">
      </div>
    </td>

    <td style="border-left: 1px solid #000000; width: 1px; padding: 0;"></td>

    <td style="padding-left: 18px; vertical-align: middle; color: ${primaryText};">
      <div style="margin-bottom: 10px;">
        <span style="font-size: 18px; font-weight: 700; color: ${primaryText}; display:block; line-height: 1.18; letter-spacing: 0;">${safeName}</span>
        <span style="font-size: 14px; color: ${primaryText}; display:block; line-height: 1.28; letter-spacing: 0;">${safeTitle}</span>
        <span style="font-size: 16px; font-weight: 700; color: ${primaryText}; display:block; line-height: 1.25; letter-spacing: 0; margin-top: 2px;">Linkup Management LLC</span>
      </div>

      <table cellpadding="0" cellspacing="0" border="0" style="font-size: 13px; color: ${primaryText}; border-collapse: collapse; letter-spacing: 0;">
        <tr>
          <td style="vertical-align: middle; padding-right: 7px; padding-bottom: 6px;">${phoneIcon}</td>
          <td style="vertical-align: middle; padding-right: 8px; padding-bottom: 6px; color: ${primaryText}; white-space: nowrap;">${safePhone}</td>
          <td style="vertical-align: middle; padding: 0 8px 6px 0; color: ${secondaryText};">|</td>
          <td style="vertical-align: middle; padding-right: 7px; padding-bottom: 6px;">${globeIcon}</td>
          <td style="vertical-align: middle; padding-bottom: 6px; white-space: nowrap;"><a href="${safeWebsiteHref}" style="color: ${primaryText}; text-decoration: none; letter-spacing: 0;">${safeWebsiteText}</a></td>
        </tr>
        <tr>
          <td style="vertical-align: middle; padding-right: 7px; padding-bottom: 6px;">${mailIcon}</td>
          <td colspan="4" style="vertical-align: middle; padding-bottom: 6px; white-space: nowrap;"><a href="mailto:${mailtoEmail}" style="color: ${primaryText}; text-decoration: none; letter-spacing: 0;">${safeEmailText}</a></td>
        </tr>
        <tr>
          <td style="vertical-align: middle; padding-right: 7px;">${pinIcon}</td>
          <td colspan="4" style="vertical-align: middle; color: ${primaryText}; letter-spacing: 0;">${safeAddress}</td>
        </tr>
      </table>
    </td>
  </tr>
</table>
</body>
</html>`;
    }

    function render() {
      const html = buildSignatureHTML({
        name: nameEl.value,
        title: titleEl.value,
        phone: phoneEl.value,
        email: emailEl.value,
        website: websiteEl.value,
        address: addressEl.value
      });

      outputEl.value = html;

      const doc = new DOMParser().parseFromString(html, 'text/html');
      const table = doc.querySelector('table');
      previewEl.innerHTML = '';
      if (table) previewEl.appendChild(table);
    }

    function showStatus(text) {
      statusEl.textContent = text;
      statusEl.classList.add('show');
      window.clearTimeout(showStatus._t);
      showStatus._t = window.setTimeout(() => statusEl.classList.remove('show'), 1400);
    }

    async function copyHTML() {
      outputEl.select();
      outputEl.setSelectionRange(0, outputEl.value.length);
      await navigator.clipboard.writeText(outputEl.value);
      showStatus('Copied ✅');
    }

    async function copyFormatted() {
      const html = outputEl.value;
      const doc = new DOMParser().parseFromString(html, 'text/html');
      const table = doc.querySelector('table');
      const fragment = table ? table.outerHTML : html;

      try {
        const item = new ClipboardItem({
          'text/html': new Blob([fragment], { type: 'text/html' }),
          'text/plain': new Blob([fragment], { type: 'text/plain' }),
        });
        await navigator.clipboard.write([item]);
        showStatus('Copied ✅');
      } catch (e) {
        const temp = document.createElement('div');
        temp.setAttribute('contenteditable', 'true');
        temp.style.position = 'fixed';
        temp.style.left = '-9999px';
        temp.style.top = '0';
        temp.innerHTML = fragment;
        document.body.appendChild(temp);

        const range = document.createRange();
        range.selectNodeContents(temp);
        const sel = window.getSelection();
        sel.removeAllRanges();
        sel.addRange(range);

        document.execCommand('copy');
        document.body.removeChild(temp);
        showStatus('Copied ✅');
      }
    }

    function resetAll() {
      nameEl.value = '';
      titleEl.value = '';
      phoneEl.value = '';
      emailEl.value = '';
      websiteEl.value = '';
      addressEl.value = '';
      render();
    }

    ['input', 'change'].forEach((evt) => {
      nameEl.addEventListener(evt, render);
      titleEl.addEventListener(evt, render);
      phoneEl.addEventListener(evt, render);
      emailEl.addEventListener(evt, render);
      websiteEl.addEventListener(evt, render);
      addressEl.addEventListener(evt, render);
    });

    el('copyBtn').addEventListener('click', () => copyHTML().catch(() => showStatus('Copy failed')));
    el('copyRichBtn').addEventListener('click', () => copyFormatted().catch(() => showStatus('Copy failed')));
    el('resetBtn').addEventListener('click', resetAll);

    // boot
    resetAll();
  </script>
</body>
</html>
