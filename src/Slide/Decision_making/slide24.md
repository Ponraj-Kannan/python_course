---
transition: slide-up
---

<!-- ═══════════════════════════════════════════════════════
     SLIDE 26 — MATCH CASE WITH MULTIPLE VALUES
═══════════════════════════════════════════════════════ -->

<Slide2 topic="Decision-making statements">
  <template #content>
<div class="slide-h1" style="margin-bottom:12px;">match-case — <span class="highlight">Multiple Values</span> per Case</div>

<div class="g2" style="gap:14px;">

<div class="flex-col" style="gap:10px;">
  <div v-click class="callout callout-info">
    <div style="font-size:.78rem;line-height:1.6;color:var(--slate);">
      You can match <strong style="color:var(--yellow);">multiple values</strong> in a single case using the <strong style="color:var(--green);">| (pipe)</strong> operator — like saying "match this OR that".
    </div>
  </div>
</div>

<div class="flex-col" style="gap:10px;">
<div v-click style="background:#f7f8fc;border:1px solid #e2e6f0;border-radius:10px;padding:14px 18px;font-family:'Fira Code',monospace;font-variant-ligatures:none;font-size:.74rem;line-height:1.9;color:#1e293b;">
    <span style="color:#0e6ead;">day</span> = <span style="color:#2d7a00;">"Saturday"</span><br><br>
    <span style="color:#c2410c;">match</span> <span style="color:#0e6ead;">day</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#c2410c;">case</span> <span style="color:#2d7a00;">"Saturday"</span> <span style="color:#b45309;">|</span> <span style="color:#2d7a00;">"Sunday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"🎉 It's the weekend!"</span>)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#c2410c;">case</span> <span style="color:#2d7a00;">"Monday"</span> <span style="color:#b45309;">|</span> <span style="color:#2d7a00;">"Friday"</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"📅 Start/end of week"</span>)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#c2410c;">case</span> <span style="color:#b45309;">_</span>:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#0f766e;">print</span>(<span style="color:#2d7a00;">"💼 Regular weekday"</span>)
  </div>

  <div v-click class="output-box">
    <span class="prompt">day = "Saturday" → </span>🎉 It's the weekend!<br>
    <span class="prompt">day = "Tuesday"  → </span>💼 Regular weekday
  </div>
</div>

</div>
  </template>
</Slide2>
