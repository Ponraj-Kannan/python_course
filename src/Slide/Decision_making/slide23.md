---
transition: slide-up
---

<!-- ═══════════════════════════════════════════════════════
     SLIDE 25 — IF-ELIF-ELSE vs MATCH-CASE COMPARISON
═══════════════════════════════════════════════════════ -->

<Slide2 topic="Decision-making statements">
  <template #content>
<div class="slide-h1" style="margin-bottom:14px;">if-elif-else  <span class="highlight">vs</span>  match-case</div>

<div class="g2" style="gap:14px;">

<div class="flex-col" style="gap:8px;">
  <div class="pill pill-red" style="margin-bottom:4px;border: 1px solid #bc2f41ff;">if-elif-else Approach</div>
  <div v-click style="background:#f7f8fc;border:1px solid #e2e6f0;border-radius:10px;padding:12px 18px;font-family:'Fira Code',monospace;font-variant-ligatures:none;font-size:.72rem;line-height:1.85;color:#1e293b;">
    <span style="color:#0e6ead;">day</span> = <span style="color:#2d7a00;">"Monday"</span><br><br>
    <span style="color:#c2410c;">if</span>   <span style="color:#0e6ead;">day</span> == <span style="color:#2d7a00;">"Monday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Start of work week"</span>)<br>
    <span style="color:#c2410c;">elif</span> <span style="color:#0e6ead;">day</span> == <span style="color:#2d7a00;">"Friday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Weekend soon!"</span>)<br>
    <span style="color:#c2410c;">elif</span> <span style="color:#0e6ead;">day</span> == <span style="color:#2d7a00;">"Sunday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Rest day"</span>)<br>
    <span style="color:#c2410c;">else</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Weekday"</span>)
  </div>
</div>

<div class="flex-col" style="gap:8px;">
  <div  class="pill pill-green" style="margin-bottom:4px; border: 1px solid #168b53ff;">match-case Approach</div>
  <div v-click style="background:#f7f8fc;border:1px solid #e2e6f0;border-radius:10px;padding:12px 18px;font-family:'Fira Code',monospace;font-variant-ligatures:none;font-size:.72rem;line-height:1.85;color:#1e293b;">
    <span style="color:#0e6ead;">day</span> = <span style="color:#2d7a00;">"Monday"</span><br><br>
    <span style="color:#c2410c;">match</span> <span style="color:#0e6ead;">day</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#c2410c;">case</span> <span style="color:#2d7a00;">"Monday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Start of work week"</span>)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#c2410c;">case</span> <span style="color:#2d7a00;">"Friday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Weekend soon!"</span>)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#c2410c;">case</span> <span style="color:#2d7a00;">"Sunday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Rest day"</span>)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#c2410c;">case</span> <span style="color:#b45309;">_</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"Weekday"</span>)
  </div>
</div>

</div>

<div style="margin-top:10px;">
  <table class="cmp-table">
    <thead>
      <tr v-click>
        <th>Feature</th>
        <th>if-elif-else</th>
        <th>match-case</th>
      </tr>
    </thead>
    <tbody>
      <tr v-click>
        <td>Python version</td>
        <td>All versions</td>
        <td class="yes">3.10+ only</td>
      </tr>
      <tr v-click>
        <td>Range conditions (>, &lt;)</td>
        <td class="yes">✅ Yes</td>
        <td class="no">❌ Not directly</td>
      </tr>
      <tr v-click>
        <td>Exact value matching</td>
        <td>✅ Yes</td>
        <td class="yes">✅ Cleaner syntax</td>
      </tr>
      <tr v-click>
        <td>Default handler</td>
        <td><code>else:</code></td>
        <td class="yes"><code>case _:</code></td>
      </tr>
      <tr v-click>
        <td>Best for</td>
        <td>Complex conditions, ranges</td>
        <td class="yes">Multiple exact values</td>
      </tr>
    </tbody>
  </table>
</div>
  </template>
</Slide2>
