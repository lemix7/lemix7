```aura width=800 height=360
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#000000', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes orb-a { 0%, 100% { transform: translate(0, 0); opacity: 0.6; } 50% { transform: translate(28px, -22px); opacity: 0.9; } }
    @keyframes orb-b { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(-22px, 18px); opacity: 0.75; } }
    @keyframes orb-c { 0%, 100% { transform: translate(0, 0); opacity: 0.35; } 50% { transform: translate(16px, -28px); opacity: 0.6; } }
    @keyframes ring-blink { 0%, 100% { opacity: 0.06; } 50% { opacity: 0.18; } }
    @keyframes ring-blink-b { 0%, 100% { opacity: 0.04; } 50% { opacity: 0.12; } }
    @keyframes dot-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    #hero-o1 { animation: orb-a 9s ease-in-out infinite; }
    #hero-o2 { animation: orb-b 11s ease-in-out infinite 0.8s; }
    #hero-o3 { animation: orb-a 8s ease-in-out infinite 2s; }
    #hero-o4 { animation: orb-b 13s ease-in-out infinite 0.4s; }
    #hero-o5 { animation: orb-c 7s ease-in-out infinite 1.2s; }
    #hr1 { animation: ring-blink 8s ease-in-out infinite; }
    #hr2 { animation: ring-blink 8s ease-in-out infinite 1.4s; }
    #hr3 { animation: ring-blink-b 8s ease-in-out infinite 2.8s; }
    #hr4 { animation: ring-blink-b 8s ease-in-out infinite 4.2s; }
    #hr5 { animation: ring-blink-b 10s ease-in-out infinite 5.6s; }
    #hero-dot { animation: dot-spin 20s linear infinite; }
  `}</style>

  <svg width="800" height="360" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(55,78,100,0.55)" />
        <stop offset="100%" stopColor="rgba(55,78,100,0)" />
      </radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(60,67,75,0.5)" />
        <stop offset="100%" stopColor="rgba(60,67,75,0)" />
      </radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(70,80,90,0.35)" />
        <stop offset="100%" stopColor="rgba(70,80,90,0)" />
      </radialGradient>
      <radialGradient id="hg4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(239,238,236,0.28)" />
        <stop offset="100%" stopColor="rgba(239,238,236,0)" />
      </radialGradient>
      <radialGradient id="hg5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(45,55,65,0.3)" />
        <stop offset="100%" stopColor="rgba(45,55,65,0)" />
      </radialGradient>
    </defs>
    <ellipse id="hero-o1" cx="110" cy="310" rx="260" ry="200" fill="url(#hg1)" />
    <ellipse id="hero-o2" cx="710" cy="70" rx="230" ry="190" fill="url(#hg2)" />
    <ellipse id="hero-o3" cx="620" cy="330" rx="200" ry="160" fill="url(#hg3)" />
    <ellipse id="hero-o4" cx="200" cy="55" rx="190" ry="150" fill="url(#hg4)" />
    <ellipse id="hero-o5" cx="400" cy="340" rx="170" ry="130" fill="url(#hg5)" />
    <circle id="hr1" cx="400" cy="178" r="52"  fill="none" stroke="rgba(239,238,236,0.9)" strokeWidth="0.7" />
    <circle id="hr2" cx="400" cy="178" r="92"  fill="none" stroke="rgba(239,238,236,0.9)" strokeWidth="0.7" />
    <circle id="hr3" cx="400" cy="178" r="138" fill="none" stroke="rgba(239,238,236,0.9)" strokeWidth="0.7" />
    <circle id="hr4" cx="400" cy="178" r="192" fill="none" stroke="rgba(239,238,236,0.9)" strokeWidth="0.7" />
    <circle id="hr5" cx="400" cy="178" r="256" fill="none" stroke="rgba(239,238,236,0.9)" strokeWidth="0.7" />
    <g id="hero-dot">
      <circle cx="400" cy="126" r="2.5" fill="rgba(239,238,236,0.5)" />
    </g>
  </svg>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
    <span style={{ fontSize: 52, fontWeight: 700, color: '#efeeec', letterSpacing: -2, lineHeight: 1 }}>AHMAD ALOSAYLI</span>
    <span style={{ fontSize: 13, color: '#a3a3a3', marginTop: 16, letterSpacing: 5, textTransform: 'uppercase', fontWeight: 300 }}>FULLSTACK · DEVELOPER</span>
    <div style={{ display: 'flex', gap: 8, marginTop: 30 }}>
      <span style={{ padding: '5px 16px', background: '#141414', color: '#b5b5b5', borderRadius: 100, fontSize: 11, border: '1px solid rgba(239,238,236,0.09)', letterSpacing: 1 }}>TypeScript</span>
      <span style={{ padding: '5px 16px', background: '#141414', color: '#b5b5b5', borderRadius: 100, fontSize: 11, border: '1px solid rgba(239,238,236,0.09)', letterSpacing: 1 }}>Python</span>
      <span style={{ padding: '5px 16px', background: '#141414', color: '#b5b5b5', borderRadius: 100, fontSize: 11, border: '1px solid rgba(239,238,236,0.09)', letterSpacing: 1 }}>React</span>
    </div>
  </div>
</div>
```

```aura width=800 height=220
<div style={{ display: 'flex', gap: 16, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', width: 564, padding: '28px 32px', background: '#000000', border: '1px solid #262626', borderRadius: 20, overflow: 'hidden' }}>
<svg width="564" height="220" style={{ position: 'absolute', top: 0, left: 0 }}><defs><radialGradient id="about-green"><stop offset="0%" stopColor="#66B3FF" stopOpacity="0.22"/><stop offset="100%" stopColor="#66B3FF" stopOpacity="0"/></radialGradient></defs><ellipse cx="100" cy="150" rx="230" ry="180" fill="url(#about-green)"><animate attributeName="opacity" values="0.5;1;0.5" dur="9s" repeatCount="indefinite"/></ellipse><circle cx="120" cy="110" r="72" fill="none" stroke="#efeeec" strokeOpacity="0.12"/><circle cx="120" cy="110" r="100" fill="none" stroke="#efeeec" strokeOpacity="0.07"/></svg>
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column' }}><span style={{ fontSize: 11, letterSpacing: 3, color: '#a3a3a3', marginBottom: 12 }}>ABOUT</span><span style={{ fontSize: 28, fontWeight: 600, color: '#efeeec', lineHeight: 1.2 }}>Ahmad Alosayli</span><span style={{ fontSize: 28, fontWeight: 600, color: '#efeeec', lineHeight: 1.2 }}>Full-stack developer.</span><span style={{ fontSize: 13, color: '#b5b5b5', marginTop: 16 }}>I build web apps, backend APIs, and AI tools./span><span style={{ fontSize: 12, color: '#a3a3a3', marginTop: 8 }}>Working with TypeScript, Python, React, and Express.</span></div>
</div>
<div style={{ display: 'flex', flexDirection: 'column', gap: 16, width: 220 }}>
<div style={{ display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", height: 102, borderRadius: 16, border: "1px solid #333333", background: "linear-gradient(135deg,#1f1f1f,#0c0c0c,#141414)", color: "#efeeec" }}><span style={{ fontSize: 9, color: "#a3a3a3", letterSpacing: 2, marginBottom: 8 }}>PORTFOLIO</span><span style={{ fontSize: 16, fontWeight: 600 }}>Explore my work</span><span style={{ fontSize: 10, color: "#b5b5b5", marginTop: 7 }}>ahmadalosayli.com</span></div>
<div style={{ display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", height: 102, borderRadius: 16, border: "1px solid #333333", background: "linear-gradient(135deg,#1f1f1f,#0c0c0c,#141414)", color: "#efeeec" }}><span style={{ fontSize: 9, color: "#a3a3a3", letterSpacing: 2, marginBottom: 8 }}>GITHUB</span><span style={{ fontSize: 16, fontWeight: 600 }}>Follow the code</span><span style={{ fontSize: 10, color: "#b5b5b5", marginTop: 7 }}>@lemix7</span></div>
</div></div>
```

```aura width=800 height=200
<div style={{ position: "relative", display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: "32px 40px", width: "100%", height: "100%", background: "#000000", borderRadius: 20, overflow: "hidden", fontFamily: "Inter, sans-serif", border: "1px solid #262626" }}>
<svg width="800" height="200" style={{ position: "absolute", top: 0, left: 0 }}><defs><radialGradient id="glow"><stop offset="0%" stopColor="#66B3FF" stopOpacity="0.2"/><stop offset="100%" stopColor="#66B3FF" stopOpacity="0"/></radialGradient><radialGradient id="violet"><stop offset="0%" stopColor="#404b58" stopOpacity="0.18"/><stop offset="100%" stopColor="#404b58" stopOpacity="0"/></radialGradient></defs><ellipse cx="70" cy="180" rx="260" ry="180" fill="url(#glow)"><animate attributeName="opacity" values="0.5;1;0.5" dur="9s" repeatCount="indefinite"/></ellipse><ellipse cx="740" cy="20" rx="240" ry="180" fill="url(#violet)"/></svg>
<div style={{ position: "relative", display: "flex", flexDirection: "column" }}><span style={{ fontSize: 11, letterSpacing: 4, color: "#a3a3a3", marginBottom: 18 }}>STACK</span><span style={{ fontSize: 22, fontWeight: 600, color: "#efeeec", marginBottom: 18 }}>Tools behind the work.</span><div style={{ display: "flex", flexWrap: "wrap", gap: 10 }}><span style={{ padding: "9px 18px", borderRadius: 100, border: "1px solid #333333", background: "#141414", fontSize: 14, color: "#efeeec" }}>TypeScript</span><span style={{ padding: "9px 18px", borderRadius: 100, border: "1px solid #333333", background: "#141414", fontSize: 14, color: "#efeeec" }}>Python</span><span style={{ padding: "9px 18px", borderRadius: 100, border: "1px solid #333333", background: "#141414", fontSize: 14, color: "#efeeec" }}>React</span><span style={{ padding: "9px 18px", borderRadius: 100, border: "1px solid #333333", background: "#141414", fontSize: 14, color: "#efeeec" }}>Express</span><span style={{ padding: "9px 18px", borderRadius: 100, border: "1px solid #333333", background: "#141414", fontSize: 14, color: "#efeeec" }}>FastAPI</span><span style={{ padding: "9px 18px", borderRadius: 100, border: "1px solid #333333", background: "#141414", fontSize: 14, color: "#efeeec" }}>PostgreSQL</span></div></div></div>
```

