<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Todo App — Front Complet</title>
  <style>
    /* ===========================
       THEME & LAYOUT
       =========================== */
    :root {
      --bg: #0f172a;
      --card: #0b1220;
      --muted: #94a3b8;
      --text: #e5e7eb;
      --accent: #3b82f6;
      --accent-600: #2563eb;
      --danger: #ef4444;
      --success: #10b981;
      --glass: rgba(255,255,255,0.03);
      --ring: rgba(59,130,246,.18);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;
      background:
        radial-gradient(800px 400px at 85% -10%, rgba(59,130,246,.12), transparent 40%),
        radial-gradient(700px 300px at -10% 110%, rgba(34,197,94,.06), transparent 30%),
        var(--bg);
      color:var(--text);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:20px;
    }
    .container{max-width:1100px;margin:0 auto}
    header{display:flex;justify-content:space-between;align-items:center;margin-bottom:18px;gap:12px}
    .brand{font-weight:700;font-size:18px}
    .tag{background:rgba(59,130,246,.12);padding:6px 10px;border-radius:999px;color:#bfdbfe;font-size:13px;border:1px solid rgba(59,130,246,.18)}
    .row{display:flex;gap:12px;align-items:center;flex-wrap:wrap}
    .muted{color:var(--muted);font-size:13px}
    .card{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent 60%), var(--card);
      border:1px solid rgba(148,163,184,.06);
      border-radius:14px;padding:18px;box-shadow:0 10px 30px rgba(0,0,0,.4);
    }
    .grid{display:grid;gap:16px}
    @media(min-width:900px){.grid-2{grid-template-columns:1fr 1fr}}
    input,select,textarea,button{
      background:#071126;color:var(--text);border:1px solid rgba(148,163,184,.06);
      padding:10px 12px;border-radius:10px;font:inherit;
    }
    input:focus,select:focus,textarea:focus{box-shadow:0 0 0 6px var(--ring);border-color:var(--accent)}
    button{background:var(--accent);color:white;border:none;cursor:pointer;padding:10px 12px;border-radius:10px}
    button.btn-outline{background:transparent;border:1px solid rgba(148,163,184,.06);color:var(--text)}
    button.btn-danger{background:var(--danger)}
    button.btn-success{background:var(--success)}
    h2{margin:0 0 6px}
    .spacer{height:10px}
    table{width:100%;border-collapse:collapse}
    th,td{padding:10px;border-bottom:1px solid rgba(148,163,184,.04);text-align:left;font-size:14px}
    th{color:#cbd5e1;font-weight:600}
    .pill{padding:4px 8px;border-radius:999px;border:1px solid rgba(148,163,184,.06);font-size:12px}
    .pill.high{color:#fecaca;border-color:rgba(239,68,68,.2)}
    .pill.medium{color:#fde68a;border-color:rgba(245,158,11,.18)}
    .pill.low{color:#bbf7d0;border-color:rgba(34,197,94,.18)}
    .status{font-size:12px;padding:4px 8px;border-radius:6px;border:1px dashed rgba(148,163,184,.06)}
    .hidden{display:none !important}
    .center{text-align:center}
    .small{font-size:13px;padding:6px 10px;border-radius:8px}
    .controls{display:flex;gap:10px;align-items:center;flex-wrap:wrap}
    .search{min-width:180px}
    .footer{color:var(--muted);text-align:center;margin-top:18px;font-size:13px}
    /* responsive tweaks */
    @media(max-width:640px){
      header{flex-direction:column;align-items:flex-start}
      .grid-2{grid-template-columns:1fr}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="row">
        <div class="brand">🧩 Gestion des tâches</div>
        <div class="tag">Front HTML/CSS/JS</div>
      </div>
      <div class="row">
        <div id="whoami" class="muted"></div>
        <button id="btnLogout" class="btn-outline hidden small">Se déconnecter</button>
      </div>
    </header>

    <!-- AUTH area -->
    <div id="authSection" class="grid grid-2">
      <div class="card" id="loginCard">
        <h2>Connexion</h2>
        <div class="spacer"></div>
        <form id="loginForm" class="grid">
          <input id="loginEmail" type="email" placeholder="Email" required />
          <input id="loginPassword" type="password" placeholder="Mot de passe" required />
          <div class="controls">
            <button type="submit">Se connecter</button>
            <button id="btnToRegister" type="button" class="btn-outline small">Créer un compte</button>
          </div>
          <p class="muted small">Compte admin seed: <b>admin@example.com</b> / <b>Admin@123</b></p>
        </form>
      </div>

      <div class="card" id="registerCard">
        <h2>Inscription</h2>
        <div class="spacer"></div>
        <form id="registerForm" class="grid">
          <input id="regName" type="text" placeholder="Nom" required />
          <input id="regEmail" type="email" placeholder="Email" required />
          <input id="regPassword" type="password" placeholder="Mot de passe" required />
          <div class="controls">
            <button type="submit" class="btn-success">Créer mon compte</button>
            <button id="btnToLogin" type="button" class="btn-outline small">J'ai déjà un compte</button>
          </div>
          <p class="muted small">Les nouveaux comptes ont le rôle <b>member</b> par défaut.</p>
        </form>
      </div>
    </div>

    <!-- DASHBOARDS -->
    <div id="dashboards" class="grid hidden">

      <!-- USER DASH -->
      <section id="userDash" class="card">
        <div style="display:flex;justify-content:space-between;align-items:center;gap:10px">
          <div>
            <h2>Espace membre — Mes tâches</h2>
            <div class="muted small">Créer, filtrer, modifier le statut ou supprimer vos tâches.</div>
          </div>
          <div class="controls">
            <select id="filterStatus" class="small">
              <option value="">Statut (tous)</option>
              <option value="todo">À faire</option>
              <option value="in_progress">En cours</option>
              <option value="done">Terminée</option>
            </select>
            <select id="filterPriority" class="small">
              <option value="">Priorité (toutes)</option>
              <option value="high">Haute</option>
              <option value="medium">Moyenne</option>
              <option value="low">Basse</option>
            </select>
            <input id="searchInput" class="search small" placeholder="Rechercher titre..." />
          </div>
        </div>

        <div class="spacer"></div>

        <form id="taskForm" class="controls" style="margin-bottom:12px">
          <input id="taskTitle" placeholder="Titre de la tâche" required />
          <input id="taskDesc" placeholder="Description" />
          <select id="taskPriority" class="small">
            <option value="medium">Priorité : Moyenne</option>
            <option value="high">Haute</option>
            <option value="low">Basse</option>
          </select>
          <button type="submit">➕ Ajouter</button>
        </form>

        <div style="overflow:auto">
          <table id="userTasksTbl">
            <thead><tr><th>Titre</th><th>Description</th><th>Priorité</th><th>Statut</th><th>Actions</th></tr></thead>
            <tbody></tbody>
          </table>
        </div>
      </section>

      <!-- ADMIN DASH (visible only for admins) -->
      <section id="adminDash" class="card hidden">
        <div style="display:flex;justify-content:space-between;align-items:center;gap:10px">
          <div>
            <h2>Espace admin — Utilisateurs & dernières tâches</h2>
            <div class="muted small">Gérer utilisateurs et voir les tâches globales.</div>
          </div>
          <div class="controls">
            <button id="btnRefreshAdmin" class="btn-outline">Actualiser</button>
          </div>
        </div>

        <div class="spacer"></div>
        <div class="grid grid-2">
          <div>
            <h3>Utilisateurs</h3>
            <div style="overflow:auto">
              <table id="usersTbl">
                <thead><tr><th>Nom</th><th>Email</th><th>Rôle</th></tr></thead>
                <tbody></tbody>
              </table>
            </div>
          </div>
          <div>
            <h3>Dernières tâches</h3>
            <div style="overflow:auto">
              <table id="tasksTbl">
                <thead><tr><th>Titre</th><th>Propriétaire</th><th>Priorité</th><th>Statut</th></tr></thead>
                <tbody></tbody>
              </table>
            </div>
          </div>
        </div>
      </section>

    </div>

    <div class="footer">© Gestion des tâches — Front léger</div>
  </div>

  <script>
  /* ===========================
     CONFIG → remplace cette URL
     =========================== */
  const API_BASE_URL = "https://backendgestiontaches1.onrender.com"; // <-- remplace par ton backend Render (ex: https://projet-final.onrender.com)

  /* ===========================
     ÉTAT
     =========================== */
  const state = { user: null, token: null };

  /* ===========================
     HELPERS DOM & SESSION
     =========================== */
  const $ = (sel) => document.querySelector(sel);
  const $$ = (sel) => Array.from(document.querySelectorAll(sel));

  function saveSession(user, token){
    state.user = user; state.token = token;
    localStorage.setItem('user', JSON.stringify(user));
    localStorage.setItem('token', token);
    renderTopbar();
  }
  function loadSession(){
    try {
      const u = JSON.parse(localStorage.getItem('user'));
      const t = localStorage.getItem('token');
      if (u && t) { state.user = u; state.token = t; }
    } catch {}
    renderTopbar();
  }
  function clearSession(){ localStorage.removeItem('user'); localStorage.removeItem('token'); state.user=null; state.token=null; renderUI(); }

  function renderTopbar(){
    const who = $('#whoami'), logout = $('#btnLogout');
    if (state.user) { who.textContent = `Connecté : ${state.user.name} (${state.user.role})`; logout.classList.remove('hidden'); }
    else { who.textContent = ''; logout.classList.add('hidden'); }
  }

  async function apiFetch(path, options = {}){
    const headers = Object.assign({'Content-Type':'application/json'}, options.headers || {});
    if (state.token) headers['Authorization'] = `Bearer ${state.token}`;
    const res = await fetch(API_BASE_URL + path, {...options, headers});
    if (!res.ok) {
      let msg = `HTTP ${res.status}`;
      try { const d = await res.json(); msg = d.message || JSON.stringify(d); } catch(e){}
      throw new Error(msg);
    }
    // try parse json
    try { return await res.json(); } catch { return null; }
  }

  function escapeHtml(s){
    return String(s || '').replace(/[&<>"']/g, c => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":"&#39;"}[c]));
  }

  /* ===========================
     AUTH HANDLERS
     =========================== */
  async function handleLogin(e){
    e && e.preventDefault();
    const email = $('#loginEmail').value.trim();
    const password = $('#loginPassword').value.trim();
    if(!email||!password) return alert('Remplis email + mot de passe');
    try {
      const data = await apiFetch('/auth/login', { method:'POST', body: JSON.stringify({ email, password }) });
      if (!data || !data.token) throw new Error('Réponse invalide du serveur');
      saveSession(data.user, data.token);
      renderUI();
    } catch (err){ alert('Erreur login : ' + err.message); }
  }

  async function handleRegister(e){
    e && e.preventDefault();
    const name = $('#regName').value.trim();
    const email = $('#regEmail').value.trim();
    const password = $('#regPassword').value.trim();
    if(!name||!email||!password) return alert('Remplis tous les champs');
    try {
      const data = await apiFetch('/auth/register', { method:'POST', body: JSON.stringify({ name, email, password }) });
      // si le back renvoie token + user on se log automatique, sinon on demande connexion
      if (data && data.token) {
        saveSession(data.user, data.token);
        renderUI();
      } else {
        alert('Compte créé. Connecte-toi.');
      }
    } catch (err){ alert('Erreur inscription : ' + err.message); }
  }

  /* ===========================
     USER TASKS
     =========================== */
  async function loadUserTasks(){
    try {
      const status = $('#filterStatus').value;
      const priority = $('#filterPriority').value;
      const q = $('#searchInput').value.trim();
      const params = new URLSearchParams();
      if (status) params.append('status', status);
      if (priority) params.append('priority', priority);
      if (q) params.append('q', q);
      // Ton backend user route: GET /user/tasks
      const data = await apiFetch('/user/tasks?' + params.toString());
      // Le format peut être { page, items } ou un tableau; on gère les 2.
      const tasks = Array.isArray(data) ? data : (data.items || data.tasks || []);
      const tbody = $('#userTasksTbl tbody');
      tbody.innerHTML = '';
      tasks.forEach(t => tbody.appendChild(taskRow(t)));
    } catch (err){ alert('Erreur chargement tâches : ' + err.message); }
  }

  function taskRow(t){
    const tr = document.createElement('tr');
    tr.innerHTML = `
      <td>${escapeHtml(t.title)}</td>
      <td class="muted">${escapeHtml(t.description || '')}</td>
      <td><span class="pill ${t.priority}">${t.priority}</span></td>
      <td><span class="status">${t.status}</span></td>
      <td class="row">
        <button data-id="${t._id}" data-action="edit" class="small btn-outline">Modifier</button>
        <button data-id="${t._id}" data-action="toggle" class="small btn-success">Statut</button>
        <button data-id="${t._id}" data-action="delete" class="small btn-danger">Supprimer</button>
      </td>`;
    tr.querySelectorAll('button').forEach(b => b.addEventListener('click', onTaskAction));
    return tr;
  }

  async function onTaskAction(e){
    const id = e.target.dataset.id;
    const action = e.target.dataset.action;
    try {
      if (action === 'delete') {
        if (!confirm('Supprimer cette tâche ?')) return;
        await apiFetch(`/user/tasks/${id}`, { method: 'DELETE' });
      } else if (action === 'toggle') {
        // récup current status via GET (or re-load single?) -> pour simplifier on met en done
        await apiFetch(`/user/tasks/${id}`, { method: 'PUT', body: JSON.stringify({ status: 'done' }) });
      } else if (action === 'edit') {
        const newTitle = prompt('Nouveau titre (laisser vide = annuler)');
        if (!newTitle) return;
        await apiFetch(`/user/tasks/${id}`, { method: 'PUT', body: JSON.stringify({ title: newTitle }) });
      }
      await loadUserTasks();
    } catch (err){ alert('Action impossible: ' + err.message); }
  }

  async function createTask(e){
    e && e.preventDefault();
    const title = $('#taskTitle').value.trim();
    const description = $('#taskDesc').value.trim();
    const priority = $('#taskPriority').value;
    if (!title) return alert('Titre requis');
    try {
      await apiFetch('/user/tasks', { method: 'POST', body: JSON.stringify({ title, description, priority }) });
      $('#taskForm').reset();
      await loadUserTasks();
    } catch (err){ alert('Erreur création: ' + err.message); }
  }

  /* ===========================
     ADMIN
     =========================== */
  async function loadAdmin(){
    try {
      // utilisateurs
      const usersData = await apiFetch('/admin/users');
      const users = Array.isArray(usersData) ? usersData : (usersData.users || usersData.items || usersData);
      const uBody = $('#usersTbl tbody'); uBody.innerHTML = '';
      users.forEach(u => {
        const tr = document.createElement('tr');
        tr.innerHTML = `<td>${escapeHtml(u.name)}</td><td class="muted">${escapeHtml(u.email)}</td><td>${u.role}</td>`;
        uBody.appendChild(tr);
      });

      // tâches admin (globales)
      const tData = await apiFetch('/admin/tasks?limit=30');
      const tasks = Array.isArray(tData) ? tData : (tData.items || tData.tasks || []);
      const tBody = $('#tasksTbl tbody'); tBody.innerHTML = '';
      tasks.forEach(t => {
        const tr = document.createElement('tr');
        tr.innerHTML = `<td>${escapeHtml(t.title)}</td><td class="muted">${escapeHtml(t.owner?.name || t.owner)}</td><td><span class="pill ${t.priority}">${t.priority}</span></td><td>${t.status}</td>`;
        tBody.appendChild(tr);
      });
    } catch (err){ alert('Erreur admin: ' + err.message); }
  }

  /* ===========================
     UI render
     =========================== */
  function renderUI(){
    const auth = $('#authSection'), d = $('#dashboards'), adminDash = $('#adminDash'), userDash = $('#userDash');
    if (!state.user) {
      auth.classList.remove('hidden'); d.classList.add('hidden');
      $('#btnLogout').classList.add('hidden');
      return;
    }
    auth.classList.add('hidden'); d.classList.remove('hidden'); $('#btnLogout').classList.remove('hidden');
    // si admin → montrer adminDash
    if (state.user.role === 'admin') { adminDash.classList.remove('hidden'); loadAdmin().catch(err => alert(err.message)); }
    else adminDash.classList.add('hidden');
    // load user tasks
    loadUserTasks().catch(err => alert(err.message));
  }

  /* ===========================
     EVENTS binding
     =========================== */
  // forms
  $('#loginForm').addEventListener('submit', handleLogin);
  $('#registerForm').addEventListener('submit', handleRegister);
  $('#taskForm').addEventListener('submit', createTask);
  $('#btnLogout').addEventListener('click', () => { clearSession(); });
  $('#btnToRegister').addEventListener('click', () => { /* focus register card */ window.scrollTo({top:200, behavior:'smooth'}); });
  $('#btnToLogin').addEventListener('click', () => { window.scrollTo({top:20, behavior:'smooth'}); });
  $('#filterStatus').addEventListener('change', loadUserTasks);
  $('#filterPriority').addEventListener('change', loadUserTasks);
  $('#searchInput').addEventListener('input', () => { clearTimeout(window.__t); window.__t = setTimeout(loadUserTasks, 300); });
  $('#btnRefreshAdmin').addEventListener('click', (e)=>{ e.preventDefault(); loadAdmin().catch(err=>alert(err.message)); });

  // shortcut: auto-load session on start
  (function boot(){
    loadSession();
    // show proper UI if logged
    if (state.user && state.token) renderUI();
  })();

  </script>
</body>
</html>
