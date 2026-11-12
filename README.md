[index.html](https://github.com/user-attachments/files/34760403/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SpaceX Innovative Investment Strategy | Beginner's Guide for 20s-30s</title>
<script src="https://cdn.tailwindcss.com"></script>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
<style>
  body { background: #0a0a12; color: #e2e8f0; font-family: system-ui, -apple-system, sans-serif; }
  .glass { background: rgba(255,255,255,0.05); backdrop-filter: blur(12px); border: 1px solid rgba(255,255,255,0.1); }
  .metric-card:hover, .expand-card:hover { transform: translateY(-4px); border-color: #5B21B6; }
  .chart-container { position: relative; height: 380px; }
  nav a:hover { color: #a78bfa; }
  .disclosure { font-size: 0.8rem; opacity: 0.75; }
  input[type=range] { accent-color: #7c3aed; }
  .expandable { max-height: 0; overflow: hidden; transition: max-height 0.4s ease; }
  .expandable.open { max-height: 500px; }
  .timeline-item { position: relative; padding-left: 2rem; }
  .timeline-item::before { content: ''; position: absolute; left: 0; top: 0.5rem; width: 12px; height: 12px; background: #7c3aed; border-radius: 50%; }
</style>
</head>
<body class="antialiased">
<!-- Nav -->
<nav class="sticky top-0 z-50 glass border-b border-purple-900/30">
  <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
    <div class="text-xl font-bold tracking-tight">🚀 SPCX Strategy</div>
    <div class="hidden lg:flex gap-6 text-sm">
      <a href="#basics">Basics</a>
      <a href="#spacex">SpaceX</a>
      <a href="#modeler">Modeler</a>
      <a href="#calculators">Calculators</a>
      <a href="#literacy">Literacy</a>
      <a href="#risks">Risks</a>
      <a href="#start">Start</a>
    </div>
  </div>
</nav>

<!-- Hero -->
<section class="relative min-h-[70vh] flex items-center justify-center overflow-hidden">
  <div class="absolute inset-0 bg-gradient-to-br from-purple-950/40 via-black to-blue-950/30"></div>
  <div class="relative z-10 text-center max-w-4xl px-6">
    <div class="inline-block px-4 py-1 rounded-full bg-purple-600/20 text-purple-300 text-sm mb-6 border border-purple-500/30">Beginner’s Guide · Ages 20–30 · Long-Term Focus</div>
    <h1 class="text-5xl md:text-7xl font-black mb-6 leading-tight">SpaceX<br><span class="text-transparent bg-clip-text bg-gradient-to-r from-purple-400 to-blue-400">Innovative Investment Strategy</span></h1>
    <p class="text-xl text-slate-300 mb-8">Rethink first principles. Own a piece of the AI + space + manufacturing boom. Time in the market beats timing the market—especially with a category-defining innovator.</p>
    <div class="flex gap-4 justify-center flex-wrap">
      <a href="#basics" class="px-8 py-3 bg-purple-600 hover:bg-purple-500 rounded-full font-semibold transition">Start Learning</a>
      <a href="#modeler" class="px-8 py-3 border border-purple-500 hover:bg-purple-900/50 rounded-full font-semibold transition">Interactive Modeler</a>
    </div>
  </div>
</section>

<!-- Basics -->
<section id="basics" class="py-20 px-6 max-w-6xl mx-auto">
  <h2 class="text-4xl font-bold mb-4">Investing 101 — Made Simple</h2>
  <p class="text-slate-400 mb-12 max-w-2xl">You don’t need a finance degree. These three ideas compound into generational wealth when applied with patience.</p>

  <div class="grid md:grid-cols-3 gap-6 mb-16">
    <div class="glass p-6 rounded-2xl metric-card transition">
      <div class="text-3xl mb-3">📈</div>
      <h3 class="text-xl font-bold mb-2">What is a Stock?</h3>
      <p class="text-sm text-slate-300">A stock is a small ownership slice of a company. When you buy SPCX, you own a tiny piece of SpaceX’s rockets, Starlink satellites, AI compute, and future Mars missions. As the company grows, so does the value of your ownership.</p>
    </div>
    <div class="glass p-6 rounded-2xl metric-card transition">
      <div class="text-3xl mb-3">💰</div>
      <h3 class="text-xl font-bold mb-2">Compounding</h3>
      <p class="text-sm text-slate-300">Your money earns returns, then those returns earn returns. Like a snowball rolling downhill. $10,000 at 10% becomes ~$67,000 in 20 years. At 25% (possible for hyper-growth), it becomes over $860,000.</p>
    </div>
    <div class="glass p-6 rounded-2xl metric-card transition">
      <h3 class="text-xl font-bold mb-2">🔄 Dollar-Cost Averaging (DCA)</h3>
      <p class="text-sm text-slate-300">Invest a fixed amount on a regular schedule (e.g., $200 every paycheck) regardless of price. You buy more shares when prices are low and fewer when high—automatically reducing emotional timing mistakes.</p>
    </div>
  </div>

  <div class="glass p-8 rounded-2xl mb-12">
    <h3 class="text-2xl font-bold mb-4">The Power of Time in the Market</h3>
    <p class="mb-6 text-slate-300">Person A buys SPCX early and keeps adding via DCA for 20 years. Person B sells every time the stock dips 20%. History and math show Person A almost always ends with dramatically more wealth.</p>
    <div class="chart-container"><canvas id="timeChart"></canvas></div>
  </div>

  <div class="glass p-8 rounded-2xl">
    <h3 class="text-2xl font-bold mb-4">Compounding Calculator</h3>
    <div class="grid md:grid-cols-3 gap-4 mb-6">
      <div><label class="text-sm">Initial Amount ($)</label><input id="init" type="number" value="10000" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
      <div><label class="text-sm">Monthly Add ($)</label><input id="monthly" type="number" value="300" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
      <div><label class="text-sm">Annual Return %</label><input id="rate" type="number" value="15" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
    </div>
    <button onclick="calcCompound()" class="bg-purple-600 px-6 py-2 rounded-full mb-4">Calculate</button>
    <div id="compoundResult" class="text-2xl font-bold text-purple-300"></div>
    <div class="chart-container mt-6"><canvas id="compoundChart"></canvas></div>
  </div>
</section>

<!-- SpaceX Overview + Expandable Cards + Timeline -->
<section id="spacex" class="py-20 px-6 bg-gradient-to-b from-transparent to-purple-950/20">
  <div class="max-w-6xl mx-auto">
    <h2 class="text-4xl font-bold mb-4">SpaceX: A Conglomerate of Startups Under One Roof</h2>
    <p class="text-slate-400 mb-12 max-w-3xl">ARK / Cathie Wood style: SpaceX is a vertically integrated stack of high-margin businesses that reinforce each other through shared infrastructure and cost advantages.</p>

    <div class="grid md:grid-cols-2 gap-6 mb-16">
      <!-- Expandable product cards -->
      <div class="glass p-6 rounded-2xl expand-card transition cursor-pointer" onclick="toggleExpand(this)">
        <div class="flex justify-between items-center">
          <h4 class="font-bold text-purple-300 text-lg">Starlink (Connectivity)</h4>
          <span class="text-xl">+</span>
        </div>
        <p class="text-sm mt-2 text-slate-300">Global satellite broadband + emerging mobile/direct-to-cell. High recurring revenue once capacity scales.</p>
        <div class="expandable mt-4 text-sm text-slate-300">
          <strong>Flywheel:</strong> Starship lowers launch cost → more V3 satellites cheaper → higher capacity → more subscribers at competitive pricing → recurring cash that funds AI and next-gen infrastructure. Analysts have modeled paths toward tens of millions of subscribers by the early 2030s, with capacity expansion enabling further growth.
        </div>
      </div>
      <div class="glass p-6 rounded-2xl expand-card transition cursor-pointer" onclick="toggleExpand(this)">
        <div class="flex justify-between items-center">
          <h4 class="font-bold text-blue-300 text-lg">Super Intelligence (AI)</h4>
          <span class="text-xl">+</span>
        </div>
        <p class="text-sm mt-2 text-slate-300">Compute, Grok models, and applications. Already the largest revenue segment in recent quarters.</p>
        <div class="expandable mt-4 text-sm text-slate-300">
          <strong>Flywheel:</strong> Vertical integration from power/chips to models to applications reduces cost per token and improves margins as scale increases. Orbital or terrestrial compute advantages compound with Starlink distribution. This is positioned as the primary long-term value driver.
        </div>
      </div>
      <div class="glass p-6 rounded-2xl expand-card transition cursor-pointer" onclick="toggleExpand(this)">
        <div class="flex justify-between items-center">
          <h4 class="font-bold text-orange-300 text-lg">Launch / Starship</h4>
          <span class="text-xl">+</span>
        </div>
        <p class="text-sm mt-2 text-slate-300">Fully reusable heavy-lift system that collapses the cost of access to space.</p>
        <div class="expandable mt-4 text-sm text-slate-300">
          <strong>Flywheel:</strong> Higher cadence → dramatically lower cost per kg → enables massive Starlink deployment, potential orbital compute, and multiplanetary cargo. Cost curve improvements create durable advantages versus less integrated competitors.
        </div>
      </div>
      <div class="glass p-6 rounded-2xl expand-card transition cursor-pointer" onclick="toggleExpand(this)">
        <div class="flex justify-between items-center">
          <h4 class="font-bold text-green-300 text-lg">Future Layers</h4>
          <span class="text-xl">+</span>
        </div>
        <p class="text-sm mt-2 text-slate-300">Terafab chips, orbital compute, spectrum, manufacturing automation, multiplanetary infrastructure.</p>
        <div class="expandable mt-4 text-sm text-slate-300">
          <strong>Flywheel:</strong> Each new layer uses the cost advantages of the previous ones. Owning the full stack (launch + satellites + compute + chips + power) is the structural edge.
        </div>
      </div>
    </div>

    <!-- Timeline -->
    <div class="glass p-8 rounded-2xl">
      <h3 class="text-2xl font-bold mb-6">Key Milestones Timeline</h3>
      <div class="space-y-6">
        <div class="timeline-item"><strong>2002–2010s:</strong> Founding, Falcon 1, Falcon 9 development and first reusability demos.</div>
        <div class="timeline-item"><strong>2019–2025:</strong> Starlink constellation buildout, rapid subscriber growth, first profitable scale in connectivity.</div>
        <div class="timeline-item"><strong>June 2026:</strong> Historic IPO (SPCX) at $135, largest ever, combining space + AI under one public company.</div>
        <div class="timeline-item"><strong>2026–2027:</strong> AI segment becomes largest by revenue; Starship reaches orbit and begins revenue missions; compute capacity scales toward multi-GW.</div>
        <div class="timeline-item"><strong>Late 2020s–2030s (projected):</strong> Higher Starship cadence, Starlink toward tens of millions of users, AI compute as core profit engine, further vertical integration.</div>
      </div>
    </div>
  </div>
</section>

<!-- Interactive Scenario Modeler -->
<section id="modeler" class="py-20 px-6 max-w-6xl mx-auto">
  <h2 class="text-4xl font-bold mb-4">Interactive Scenario Modeler</h2>
  <p class="text-slate-400 mb-8">Adjust the sliders to explore different futures. Numbers are illustrative educational models only.</p>

  <div class="glass p-8 rounded-2xl mb-8">
    <div class="grid md:grid-cols-2 gap-8">
      <div>
        <label class="block text-sm mb-2">Starlink Annual Subscriber Growth Rate: <span id="starlinkVal">40</span>%</label>
        <input type="range" id="starlink" min="10" max="70" value="40" class="w-full" oninput="updateModeler()">
      </div>
      <div>
        <label class="block text-sm mb-2">AI Compute Scale (relative, 1–10): <span id="aiVal">6</span></label>
        <input type="range" id="ai" min="1" max="10" value="6" class="w-full" oninput="updateModeler()">
      </div>
      <div>
        <label class="block text-sm mb-2">Starship Cadence Impact (1–10): <span id="starshipVal">5</span></label>
        <input type="range" id="starship" min="1" max="10" value="5" class="w-full" oninput="updateModeler()">
      </div>
      <div>
        <label class="block text-sm mb-2">Applied Revenue Multiple: <span id="multipleVal">25</span>x</label>
        <input type="range" id="multiple" min="8" max="50" value="25" class="w-full" oninput="updateModeler()">
      </div>
    </div>
  </div>

  <div class="chart-container mb-8"><canvas id="modelerChart"></canvas></div>

  <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
    <div class="glass p-4 rounded-xl text-center"><div class="text-sm text-slate-400">5-Year Revenue</div><div id="m5" class="text-2xl font-bold text-purple-300">—</div></div>
    <div class="glass p-4 rounded-xl text-center"><div class="text-sm text-slate-400">10-Year Revenue</div><div id="m10" class="text-2xl font-bold text-purple-300">—</div></div>
    <div class="glass p-4 rounded-xl text-center"><div class="text-sm text-slate-400">15-Year Revenue</div><div id="m15" class="text-2xl font-bold text-purple-300">—</div></div>
    <div class="glass p-4 rounded-xl text-center"><div class="text-sm text-slate-400">20-Year Revenue</div><div id="m20" class="text-2xl font-bold text-purple-300">—</div></div>
  </div>
</section>

<!-- Calculators: DCA/Ownership + Goal -->
<section id="calculators" class="py-20 px-6 bg-slate-900/50">
  <div class="max-w-6xl mx-auto">
    <h2 class="text-4xl font-bold mb-4">Personal Calculators</h2>

    <!-- DCA / Ownership -->
    <div class="glass p-8 rounded-2xl mb-12">
      <h3 class="text-2xl font-bold mb-4">SPCX DCA + Ownership Calculator</h3>
      <div class="grid md:grid-cols-3 gap-4 mb-6">
        <div><label class="text-sm">Initial Investment ($)</label><input id="dcaInit" type="number" value="5000" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
        <div><label class="text-sm">Monthly Contribution ($)</label><input id="dcaMonthly" type="number" value="500" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
        <div><label class="text-sm">Years</label><input id="dcaYears" type="number" value="15" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
      </div>
      <button onclick="calcDCA()" class="bg-purple-600 px-6 py-2 rounded-full mb-4">Calculate</button>
      <div id="dcaResult" class="text-lg text-purple-300 mb-4"></div>
      <div class="chart-container"><canvas id="dcaChart"></canvas></div>
    </div>

    <!-- Goal Calculator -->
    <div class="glass p-8 rounded-2xl">
      <h3 class="text-2xl font-bold mb-4">“How Much Do I Need?” Goal Calculator</h3>
      <div class="grid md:grid-cols-3 gap-4 mb-6">
        <div><label class="text-sm">Target Portfolio Value ($)</label><input id="goalTarget" type="number" value="1000000" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
        <div><label class="text-sm">Years to Goal</label><input id="goalYears" type="number" value="20" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
        <div><label class="text-sm">Assumed Annual Return %</label><input id="goalRate" type="number" value="15" class="w-full mt-1 bg-slate-800 rounded px-3 py-2"></div>
      </div>
      <button onclick="calcGoal()" class="bg-purple-600 px-6 py-2 rounded-full mb-4">Calculate Monthly Need</button>
      <div id="goalResult" class="text-2xl font-bold text-purple-300"></div>
    </div>
  </div>
</section>

<!-- Financial Literacy -->
<section id="literacy" class="py-20 px-6 max-w-6xl mx-auto">
  <h2 class="text-4xl font-bold mb-4">Simple Financial Literacy for Innovators</h2>
  <div class="grid md:grid-cols-2 gap-8">
    <div class="glass p-6 rounded-2xl">
      <h3 class="font-bold text-lg mb-3">Why High Multiples Can Still Make Sense</h3>
      <p class="text-sm text-slate-300">A high price-to-sales (P/S) ratio is not automatically “expensive.” For a company growing revenue 50–100%+ per year while expanding its addressable market, today’s multiple can compress as revenue scales. The key questions are: Is the growth durable? Is the moat real? Can margins expand at scale? Hyper-growth companies are often valued on future cash flows, not current ones.</p>
    </div>
    <div class="glass p-6 rounded-2xl">
      <h3 class="font-bold text-lg mb-3">What to Look for in Quarterly Updates</h3>
      <ul class="text-sm text-slate-300 space-y-2">
        <li>• Starlink subscriber growth and ARPU trends</li>
        <li>• AI / Super Intelligence revenue and compute capacity (GW)</li>
        <li>• Launch cadence and Starship progress</li>
        <li>• Operating margins and free cash flow trajectory</li>
        <li>• Capex intensity vs. revenue growth</li>
      </ul>
    </div>
  </div>
</section>

<!-- Risks (Constructive) -->
<section id="risks" class="py-20 px-6 bg-slate-900/30">
  <div class="max-w-6xl mx-auto">
    <h2 class="text-4xl font-bold mb-4">Risks — And What Must Be True for the Bull Case</h2>
    <div class="grid md:grid-cols-2 gap-6">
      <div class="glass p-6 rounded-2xl">
        <h3 class="font-bold text-red-300 mb-3">Real Risks</h3>
        <ul class="text-sm text-slate-300 space-y-2">
          <li>• Execution risk on Starship cadence and reliability</li>
          <li>• AI competition and potential commoditization of compute</li>
          <li>• Capital intensity and potential dilution</li>
          <li>• Regulatory, spectrum, or geopolitical friction</li>
          <li>• Key-person dependency and valuation volatility</li>
        </ul>
      </div>
      <div class="glass p-6 rounded-2xl">
        <h3 class="font-bold text-green-300 mb-3">What Needs to Be True</h3>
        <ul class="text-sm text-slate-300 space-y-2">
          <li>• Starship reaches high, reliable cadence</li>
          <li>• Starlink continues compounding subscribers with improving unit economics</li>
          <li>• AI compute business scales with strong utilization and margins</li>
          <li>• Vertical integration continues to produce cost advantages</li>
          <li>• Management executes on multi-year capital plans without major setbacks</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- Comparisons (kept concise) -->
<section class="py-20 px-6 max-w-6xl mx-auto">
  <h2 class="text-4xl font-bold mb-4">Traditional Paths vs. High-Conviction Innovation</h2>
  <p class="text-slate-400 mb-8">Index funds, 401(k)s, and Roth IRAs are excellent foundations (especially for tax advantages and diversification). A concentrated long-term position in a category-defining innovator can produce asymmetric outcomes over decades.</p>
  <div class="chart-container"><canvas id="compareChart"></canvas></div>
</section>

<!-- Start Investing -->
<section id="start" class="py-20 px-6 bg-gradient-to-t from-purple-950/30 to-transparent">
  <div class="max-w-4xl mx-auto">
    <h2 class="text-4xl font-bold mb-4">How to Start Investing Today</h2>
    <div class="space-y-6">
      <div class="glass p-6 rounded-2xl">
        <h3 class="font-bold">1. Open a Brokerage Account</h3>
        <p class="text-sm text-slate-300 mt-2">Fidelity, Charles Schwab, Vanguard, Robinhood, or Public. Many offer $0 commissions and fractional shares so you can start with small amounts.</p>
      </div>
      <div class="glass p-6 rounded-2xl">
        <h3 class="font-bold">2. Prioritize Tax-Advantaged Accounts</h3>
        <p class="text-sm text-slate-300 mt-2">Max the employer 401(k) match first, then consider a Roth IRA. You can often hold individual stocks inside these accounts.</p>
      </div>
      <div class="glass p-6 rounded-2xl">
        <h3 class="font-bold">3. Learn to Evaluate a Company Yourself</h3>
        <p class="text-sm text-slate-300 mt-2">Read quarterly results, track the metrics above, and understand the competitive position. Don’t outsource conviction you haven’t built.</p>
      </div>
      <div class="glass p-6 rounded-2xl">
        <h3 class="font-bold">4. Dollar-Cost Average & Hold Long-Term</h3>
        <p class="text-sm text-slate-300 mt-2">Set up automatic investments. Time in the market is your biggest edge as a young investor.</p>
      </div>
    </div>
  </div>
</section>

<!-- Disclosure -->
<footer class="py-12 px-6 border-t border-slate-800">
  <div class="max-w-4xl mx-auto disclosure text-center">
    <p class="mb-4"><strong>Important Disclosure:</strong> This is not financial, investment, tax, or legal advice. It is educational content only. Past performance is not indicative of future results. SpaceX (SPCX) is a high-risk, high-volatility stock. You can lose some or all of your investment. All projections, scenarios, and calculator results are purely illustrative and hypothetical. Always do your own research (DYOR), consider your risk tolerance, and consult a qualified financial advisor if needed. Diversification is generally recommended for most investors.</p>
    <p>Interactive educational guide focused on long-term innovation investing. Figures are simplified models for learning purposes and are subject to change.</p>
  </div>
</footer>

<script>
function toggleExpand(el) {
  const exp = el.querySelector('.expandable');
  exp.classList.toggle('open');
  el.querySelector('span').textContent = exp.classList.contains('open') ? '−' : '+';
}

// Time chart
const timeCtx = document.getElementById('timeChart').getContext('2d');
new Chart(timeCtx, {
  type: 'line',
  data: {
    labels: ['Year 1','5','10','15','20'],
    datasets: [{
      label: 'Person A (DCA + Hold)',
      data: [6000, 45000, 140000, 320000, 650000],
      borderColor: '#a78bfa',
      tension: 0.3
    }, {
      label: 'Person B (Sells on Dips)',
      data: [5000, 18000, 35000, 55000, 80000],
      borderColor: '#f87171',
      tension: 0.3
    }]
  },
  options: { responsive: true, plugins: { legend: { labels: { color: '#e2e8f0' } } }, scales: { x: { ticks: { color: '#94a3b8' } }, y: { ticks: { color: '#94a3b8' } } } }
});

// Compound calculator
let compoundChart;
function calcCompound() {
  const init = +document.getElementById('init').value || 0;
  const monthly = +document.getElementById('monthly').value || 0;
  const rate = (+document.getElementById('rate').value || 0) / 100;
  const years = 20;
  let bal = init;
  const data = [Math.round(bal)];
  for (let y = 1; y <= years; y++) {
    bal = bal * (1 + rate) + monthly * 12;
    data.push(Math.round(bal));
  }
  document.getElementById('compoundResult').innerText = `After 20 years: $${data[data.length-1].toLocaleString()}`;
  if (compoundChart) compoundChart.destroy();
  const ctx = document.getElementById('compoundChart').getContext('2d');
  compoundChart = new Chart(ctx, {
    type: 'line',
    data: { labels: Array.from({length: years+1}, (_,i)=>i), datasets: [{ label: 'Portfolio Value', data, borderColor: '#c084fc', tension: 0.2 }] },
    options: { responsive: true, plugins: { legend: { labels: { color: '#e2e8f0' } } }, scales: { x: { ticks: { color: '#94a3b8' } }, y: { ticks: { color: '#94a3b8' } } } }
  });
}
calcCompound();

// Modeler
let modelerChart;
function updateModeler() {
  const starlink = +document.getElementById('starlink').value;
  const ai = +document.getElementById('ai').value;
  const starship = +document.getElementById('starship').value;
  const multiple = +document.getElementById('multiple').value;
  document.getElementById('starlinkVal').textContent = starlink;
  document.getElementById('aiVal').textContent = ai;
  document.getElementById('starshipVal').textContent = starship;
  document.getElementById('multipleVal').textContent = multiple;

  // Simplified illustrative model starting from ~$60B
  const base = 60;
  const growthFactor = (starlink/40) * 0.4 + (ai/6) * 0.4 + (starship/5) * 0.2;
  const revs = [5,10,15,20].map(y => Math.round(base * Math.pow(1 + 0.35 * growthFactor, y)));
  document.getElementById('m5').textContent = '$' + revs[0] + 'B';
  document.getElementById('m10').textContent = '$' + revs[1] + 'B';
  document.getElementById('m15').textContent = '$' + revs[2] + 'B';
  document.getElementById('m20').textContent = '$' + revs[3] + 'B';

  if (modelerChart) modelerChart.destroy();
  const ctx = document.getElementById('modelerChart').getContext('2d');
  modelerChart = new Chart(ctx, {
    type: 'line',
    data: {
      labels: ['5 Years','10 Years','15 Years','20 Years'],
      datasets: [{ label: 'Illustrative Revenue ($B)', data: revs, borderColor: '#a78bfa', tension: 0.3, pointRadius: 6 }]
    },
    options: { responsive: true, plugins: { legend: { labels: { color: '#e2e8f0' } } }, scales: { x: { ticks: { color: '#94a3b8' } }, y: { ticks: { color: '#94a3b8' } } } }
  });
}
updateModeler();

// DCA Calculator
let dcaChart;
function calcDCA() {
  const init = +document.getElementById('dcaInit').value || 0;
  const monthly = +document.getElementById('dcaMonthly').value || 0;
  const years = +document.getElementById('dcaYears').value || 15;
  const spxRate = 0.10;
  const spcxRate = 0.18; // illustrative high-growth
  let spx = init, spcx = init;
  const labels = [], spxData = [], spcxData = [];
  for (let y = 0; y <= years; y++) {
    labels.push(y);
    spxData.push(Math.round(spx));
    spcxData.push(Math.round(spcx));
    spx = spx * (1 + spxRate) + monthly * 12;
    spcx = spcx * (1 + spcxRate) + monthly * 12;
  }
  const totalContrib = init + monthly * 12 * years;
  document.getElementById('dcaResult').innerHTML = 
    `S&P 500 (~10%): $${spxData[spxData.length-1].toLocaleString()}<br>` +
    `SPCX Illustrative (~18%): $${spcxData[spcxData.length-1].toLocaleString()}<br>` +
    `Total contributed: $${totalContrib.toLocaleString()}`;

  if (dcaChart) dcaChart.destroy();
  const ctx = document.getElementById('dcaChart').getContext('2d');
  dcaChart = new Chart(ctx, {
    type: 'line',
    data: {
      labels,
      datasets: [
        { label: 'S&P 500', data: spxData, borderColor: '#64748b', tension: 0.2 },
        { label: 'SPCX Illustrative', data: spcxData, borderColor: '#a78bfa', tension: 0.2 }
      ]
    },
    options: { responsive: true, plugins: { legend: { labels: { color: '#e2e8f0' } } }, scales: { x: { ticks: { color: '#94a3b8' } }, y: { ticks: { color: '#94a3b8' } } } }
  });
}
calcDCA();

// Goal Calculator
function calcGoal() {
  const target = +document.getElementById('goalTarget').value || 0;
  const years = +document.getElementById('goalYears').value || 20;
  const rate = (+document.getElementById('goalRate').value || 0) / 100;
  if (rate <= 0 || years <= 0) return;
  // Approximate monthly payment needed (future value of annuity)
  const monthlyRate = rate / 12;
  const months = years * 12;
  const monthly = target / (((Math.pow(1 + monthlyRate, months) - 1) / monthlyRate));
  document.getElementById('goalResult').innerText = `Approximately $${Math.round(monthly).toLocaleString()} per month to reach $${target.toLocaleString()} in ${years} years at ${rate*100}% annual return.`;
}
calcGoal();

// Comparison chart
const compareCtx = document.getElementById('compareChart').getContext('2d');
new Chart(compareCtx, {
  type: 'bar',
  data: {
    labels: ['5 Years','10 Years','15 Years','20 Years'],
    datasets: [
      { label: 'S&P 500 (~10%)', data: [22000, 62000, 160000, 400000], backgroundColor: '#64748b' },
      { label: 'High-Conviction Illustrative', data: [45000, 280000, 1200000, 4500000], backgroundColor: '#a78bfa' }
    ]
  },
  options: { responsive: true, plugins: { legend: { labels: { color: '#e2e8f0' } } }, scales: { x: { ticks: { color: '#94a3b8' } }, y: { ticks: { color: '#94a3b8', callback: v => '$'+(v/1000)+'k' } } } }
});
</script>
</body>
</html>
