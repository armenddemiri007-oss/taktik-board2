import { useState, useRef, useCallback, useEffect } from "react";

const PLAYERS = {
  u17: [
    {id:1, name:'Max Müller',  num:1,  pos:'TW', pg:'gk',  age:16,foot:'R',rating:78,speed:62,tech:70,phys:74,mental:80,tags:['Reflexe','Führung'],    bench:false},
    {id:2, name:'Leo Brand',   num:2,  pos:'RV', pg:'def', age:16,foot:'R',rating:71,speed:77,tech:69,phys:68,mental:66,tags:['Überlappend'],           bench:false},
    {id:3, name:'Nico Schmid', num:4,  pos:'IV', pg:'def', age:17,foot:'R',rating:74,speed:71,tech:68,phys:76,mental:72,tags:['Zweikampf','Kopfball'],  bench:false},
    {id:4, name:'Ben Keller',  num:5,  pos:'IV', pg:'def', age:16,foot:'L',rating:72,speed:68,tech:65,phys:78,mental:70,tags:['Physis'],                bench:false},
    {id:5, name:'Jan Roos',    num:3,  pos:'LV', pg:'def', age:17,foot:'L',rating:73,speed:78,tech:71,phys:70,mental:68,tags:['Schnell','Flanken'],     bench:false},
    {id:6, name:'Elias Vogel', num:6,  pos:'DM', pg:'mid', age:16,foot:'R',rating:76,speed:70,tech:74,phys:79,mental:77,tags:['Ballgewinn'],            bench:false},
    {id:7, name:'Tim Fischer', num:8,  pos:'ZM', pg:'mid', age:17,foot:'R',rating:82,speed:74,tech:83,phys:72,mental:85,tags:['Spielmacher','Pass'],    bench:false},
    {id:8, name:'Marc Stein',  num:7,  pos:'RA', pg:'mid', age:17,foot:'R',rating:79,speed:85,tech:78,phys:68,mental:74,tags:['Dribbling','Tempo'],     bench:false},
    {id:9, name:'Jonas Weber', num:11, pos:'LA', pg:'mid', age:16,foot:'L',rating:80,speed:86,tech:77,phys:66,mental:73,tags:['Schnell','Flanken'],     bench:false},
    {id:10,name:'Finn Hess',   num:9,  pos:'ST', pg:'fwd', age:17,foot:'L',rating:81,speed:80,tech:79,phys:77,mental:78,tags:['Stärke','Pressing'],     bench:false},
    {id:11,name:'Luca Bauer',  num:10, pos:'ST', pg:'fwd', age:17,foot:'R',rating:88,speed:83,tech:85,phys:76,mental:87,tags:['Torinstinkt','Leader'],  bench:false},
    {id:12,name:'Aaron Lang',  num:12, pos:'TW', pg:'gk',  age:15,foot:'R',rating:65,speed:58,tech:60,phys:62,mental:63,tags:['Nachwuchs'],             bench:true},
    {id:13,name:'Pascal Wolf', num:14, pos:'IV', pg:'def', age:16,foot:'R',rating:68,speed:65,tech:63,phys:70,mental:66,tags:['Solide'],                bench:true},
    {id:14,name:'Robin Mayr',  num:15, pos:'MF', pg:'mid', age:15,foot:'R',rating:70,speed:73,tech:68,phys:65,mental:69,tags:['Dynamisch'],             bench:true},
    {id:15,name:'Sven Graf',   num:16, pos:'ST', pg:'fwd', age:16,foot:'R',rating:72,speed:77,tech:71,phys:68,mental:70,tags:['Joker'],                 bench:true},
  ],
  u15: [
    {id:101,name:'David Roth',   num:1, pos:'TW',pg:'gk',  age:14,foot:'R',rating:74,speed:60,tech:68,phys:70,mental:76,tags:['Reflexe'],       bench:false},
    {id:102,name:'Simon Huber',  num:2, pos:'RV',pg:'def', age:15,foot:'R',rating:67,speed:72,tech:64,phys:64,mental:65,tags:['Überlappend'],   bench:false},
    {id:103,name:'Kai Berner',   num:4, pos:'IV',pg:'def', age:15,foot:'R',rating:70,speed:68,tech:65,phys:72,mental:69,tags:['Zweikampf'],     bench:false},
    {id:104,name:'Nick Lorenz',  num:5, pos:'IV',pg:'def', age:14,foot:'R',rating:69,speed:66,tech:63,phys:71,mental:67,tags:['Physis'],        bench:false},
    {id:105,name:'Tom Pfeiffer', num:3, pos:'LV',pg:'def', age:14,foot:'L',rating:68,speed:74,tech:66,phys:65,mental:64,tags:['Flanken'],       bench:false},
    {id:106,name:'Luis Wolf',    num:6, pos:'ZM',pg:'mid', age:15,foot:'R',rating:78,speed:72,tech:79,phys:68,mental:80,tags:['Spielmacher'],   bench:false},
    {id:107,name:'Cem Yildiz',   num:8, pos:'OM',pg:'mid', age:14,foot:'R',rating:75,speed:76,tech:77,phys:65,mental:74,tags:['Kreativ'],       bench:false},
    {id:108,name:'Noah Klein',   num:7, pos:'RA',pg:'mid', age:15,foot:'R',rating:76,speed:82,tech:74,phys:64,mental:72,tags:['Tempo'],         bench:false},
    {id:109,name:'Eric Sommer',  num:11,pos:'LA',pg:'mid', age:14,foot:'L',rating:73,speed:80,tech:72,phys:62,mental:70,tags:['Schnell'],       bench:false},
    {id:110,name:'Ben Seidl',    num:10,pos:'ST',pg:'fwd', age:15,foot:'L',rating:77,speed:76,tech:75,phys:70,mental:75,tags:['Pressing'],      bench:false},
    {id:111,name:'Finn Huber',   num:9, pos:'ST',pg:'fwd', age:15,foot:'R',rating:84,speed:79,tech:81,phys:73,mental:83,tags:['Torjäger'],      bench:false},
    {id:112,name:'Nico Frei',    num:12,pos:'TW',pg:'gk',  age:13,foot:'R',rating:62,speed:55,tech:58,phys:60,mental:60,tags:['Nachwuchs'],     bench:true},
    {id:113,name:'Jannis Koch',  num:14,pos:'MF',pg:'mid', age:14,foot:'R',rating:65,speed:70,tech:63,phys:62,mental:64,tags:['Einsatz'],       bench:true},
    {id:114,name:'Milo Stark',   num:15,pos:'ST',pg:'fwd', age:13,foot:'R',rating:67,speed:74,tech:66,phys:61,mental:65,tags:['Joker'],         bench:true},
  ]
};

// Horizontal pitch: x%=left→right, y%=top→bottom. GK left, attack right.
const FORMATIONS = {
  '4-3-3':   [[8,50],[22,20],[22,40],[22,60],[22,80],[42,30],[50,50],[42,70],[72,20],[72,50],[72,80]],
  '4-4-2':   [[8,50],[22,20],[22,40],[22,60],[22,80],[44,20],[44,43],[44,57],[44,80],[65,35],[65,65]],
  '4-2-3-1': [[8,50],[22,20],[22,40],[22,60],[22,80],[38,35],[38,65],[56,20],[56,50],[56,80],[76,50]],
  '3-5-2':   [[8,50],[22,28],[22,50],[22,72],[40,15],[42,36],[50,52],[42,68],[40,85],[66,35],[66,65]],
  '3-4-3':   [[8,50],[22,28],[22,50],[22,72],[44,20],[44,43],[44,57],[44,80],[70,20],[70,50],[70,80]],
  '5-3-2':   [[8,50],[18,14],[18,32],[22,50],[18,68],[18,86],[42,28],[50,50],[42,72],[65,35],[65,65]],
};

const PG_COLORS = { gk:'#c87020', def:'#1a4fa8', mid:'#2d8a3e', fwd:'#b03030' };
const PG_BORDERS = { gk:'#f0b060', def:'#70a0f8', mid:'#70d880', fwd:'#f07878' };

function ratingColor(r) { return r>=80?'#4aba5e':r>=72?'#f0c040':'#e05555'; }

function StatBar({ value, color }) {
  return (
    <div style={{height:4,background:'rgba(255,255,255,0.08)',borderRadius:2,marginTop:5,overflow:'hidden'}}>
      <div style={{height:'100%',width:`${value}%`,background:color,borderRadius:2}} />
    </div>
  );
}

function PlayerDetail({ player, onBack }) {
  if (!player) return null;
  const attrs = [
    {n:'Tempo',  v:player.speed,  c:'#f0c040'},
    {n:'Technik',v:player.tech,   c:'#4a90d9'},
    {n:'Physis', v:player.phys,   c:'#e05555'},
    {n:'Mental', v:player.mental, c:'#4aba5e'},
  ];
  const tagClass = {Tempo:'speed',Schnell:'speed',Überlappend:'speed',Bewegung:'speed',Technik:'tech',Dribbling:'tech',Passspiel:'tech',Pass:'tech',Flanken:'tech',Kreativ:'tech',Spielmacher:'tech',Physis:'phys',Zweikampf:'phys',Kopfball:'phys',Stärke:'phys',Reflexe:'phys',Ballgewinn:'phys',Pressing:'phys',Defensiv:'phys',Leader:'mental',Führung:'mental',Torinstinkt:'mental',Torjäger:'mental'};
  const tagColors = {speed:['rgba(240,192,64,0.2)','#f0c040','rgba(240,192,64,0.35)'],tech:['rgba(74,144,217,0.2)','#4a90d9','rgba(74,144,217,0.35)'],phys:['rgba(224,85,85,0.2)','#e05555','rgba(224,85,85,0.35)'],mental:['rgba(78,186,94,0.2)','#4aba5e','rgba(78,186,94,0.35)']};
  const rc = ratingColor(player.rating);
  return (
    <div style={{padding:14}}>
      <button onClick={onBack} style={{background:'none',border:'1px solid rgba(255,255,255,0.1)',color:'#7a9a7d',fontFamily:'Barlow Condensed,sans-serif',fontSize:12,padding:'5px 10px',borderRadius:6,cursor:'pointer',marginBottom:12}}>← Zurück</button>
      <div style={{display:'flex',alignItems:'center',gap:12,marginBottom:14}}>
        <div style={{width:50,height:50,borderRadius:12,background:PG_COLORS[player.pg],display:'flex',alignItems:'center',justifyContent:'center',fontFamily:'Barlow Condensed,sans-serif',fontSize:22,fontWeight:800,color:'#fff',flexShrink:0}}>{player.num}</div>
        <div>
          <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:21,fontWeight:800,lineHeight:1}}>{player.name}</div>
          <div style={{fontSize:11,color:'#7a9a7d',marginTop:3}}>{player.pos} · {player.foot}-Fuss · {player.age} J.</div>
          <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:12,color:'#f0c040',marginTop:2}}>#{player.num}</div>
        </div>
      </div>
      <div style={{display:'grid',gridTemplateColumns:'1fr 1fr',gap:7,marginBottom:12}}>
        {[{l:'Gesamtwert',v:player.rating,c:rc},{l:'Tempo',v:player.speed,c:'#f0c040'},{l:'Technik',v:player.tech,c:'#4a90d9'},{l:'Physis',v:player.phys,c:'#e05555'}].map(s=>(
          <div key={s.l} style={{background:'#181f18',border:'1px solid rgba(255,255,255,0.08)',borderRadius:8,padding:9}}>
            <div style={{fontSize:10,color:'#7a9a7d',textTransform:'uppercase',letterSpacing:'0.5px',marginBottom:3}}>{s.l}</div>
            <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:22,fontWeight:800,color:s.c,lineHeight:1}}>{s.v}</div>
            <StatBar value={s.v} color={s.c} />
          </div>
        ))}
      </div>
      <div style={{marginBottom:11}}>
        <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:12,fontWeight:700,color:'#7a9a7d',letterSpacing:'1px',textTransform:'uppercase',marginBottom:7}}>Attribute</div>
        {attrs.map(a=>(
          <div key={a.n} style={{display:'flex',alignItems:'center',gap:8,marginBottom:5}}>
            <div style={{fontSize:11,color:'#7a9a7d',width:68,flexShrink:0}}>{a.n}</div>
            <div style={{flex:1,height:4,background:'rgba(255,255,255,0.07)',borderRadius:3,overflow:'hidden'}}>
              <div style={{height:'100%',width:`${a.v}%`,background:a.c,borderRadius:3}} />
            </div>
            <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:13,fontWeight:700,color:a.c,width:22,textAlign:'right'}}>{a.v}</div>
          </div>
        ))}
      </div>
      <div>
        <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:12,fontWeight:700,color:'#7a9a7d',letterSpacing:'1px',textTransform:'uppercase',marginBottom:7}}>Stärken</div>
        <div style={{display:'flex',gap:4,flexWrap:'wrap'}}>
          {player.tags.map(t=>{
            const cls=tagClass[t]||'mental'; const [bg,col,border]=tagColors[cls];
            return <span key={t} style={{fontSize:10,fontWeight:600,padding:'2px 7px',borderRadius:4,background:bg,color:col,border:`1px solid ${border}`}}>{t}</span>;
          })}
        </div>
      </div>
    </div>
  );
}

function Token({ player, pos, selected, onDragEnd, onClick }) {
  const ref = useRef(null);
  const dragging = useRef(false);
  const moved = useRef(false);
  const start = useRef({});

  const handleStart = useCallback((e) => {
    dragging.current = true; moved.current = false;
    const t = e.touches ? e.touches[0] : e;
    start.current = { cx: t.clientX, cy: t.clientY, px: pos.x, py: pos.y };
    e.stopPropagation();
  }, [pos]);

  const handleMove = useCallback((e) => {
    if (!dragging.current) return;
    const t = e.touches ? e.touches[0] : e;
    const dx = t.clientX - start.current.cx;
    const dy = t.clientY - start.current.cy;
    if (Math.abs(dx) > 3 || Math.abs(dy) > 3) moved.current = true;
    const pitch = ref.current?.closest('[data-pitch]');
    if (!pitch) return;
    const r = pitch.getBoundingClientRect();
    const nx = Math.max(2, Math.min(98, start.current.px + dx / r.width * 100));
    const ny = Math.max(3, Math.min(97, start.current.py + dy / r.height * 100));
    onDragEnd(player.id, nx, ny, false);
    e.preventDefault();
  }, [player.id, onDragEnd]);

  const handleEnd = useCallback(() => {
    if (!dragging.current) return;
    dragging.current = false;
    if (!moved.current) onClick(player.id);
  }, [player.id, onClick]);

  useEffect(() => {
    window.addEventListener('mousemove', handleMove, { passive: false });
    window.addEventListener('touchmove', handleMove, { passive: false });
    window.addEventListener('mouseup', handleEnd);
    window.addEventListener('touchend', handleEnd);
    return () => {
      window.removeEventListener('mousemove', handleMove);
      window.removeEventListener('touchmove', handleMove);
      window.removeEventListener('mouseup', handleEnd);
      window.removeEventListener('touchend', handleEnd);
    };
  }, [handleMove, handleEnd]);

  const bg = `linear-gradient(135deg, ${PG_COLORS[player.pg]}dd, ${PG_COLORS[player.pg]})`;
  const borderColor = selected ? '#f0c040' : PG_BORDERS[player.pg];
  const shadow = selected ? '0 0 0 2px #f0c040, 0 3px 12px rgba(0,0,0,0.7)' : '0 3px 12px rgba(0,0,0,0.7)';
  const lastName = player.name.split(' ').pop();

  return (
    <div
      ref={ref}
      onMouseDown={handleStart}
      onTouchStart={handleStart}
      style={{
        position:'absolute',
        left:`${pos.x}%`, top:`${pos.y}%`,
        transform:'translate(-50%,-50%)',
        cursor:'grab', touchAction:'none',
        zIndex: selected ? 50 : 10,
        display:'flex', flexDirection:'column', alignItems:'center', gap:2,
        width:44,
      }}
    >
      <div style={{
        width:38, height:38, borderRadius:'50%',
        background:bg,
        border:`2.5px solid ${borderColor}`,
        boxShadow:shadow,
        display:'flex', flexDirection:'column', alignItems:'center', justifyContent:'center',
      }}>
        <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:14,fontWeight:800,color:'#fff',lineHeight:1,textShadow:'0 1px 3px rgba(0,0,0,0.5)'}}>{player.num}</div>
        <div style={{fontSize:7,fontWeight:700,color:'rgba(255,255,255,0.85)',textTransform:'uppercase'}}>{player.pos}</div>
      </div>
      <div style={{fontSize:8,fontWeight:700,color:'#fff',textAlign:'center',lineHeight:1,textShadow:'0 1px 6px #000',background:'rgba(0,0,0,0.55)',padding:'1px 4px',borderRadius:3,maxWidth:48,whiteSpace:'nowrap',overflow:'hidden',textOverflow:'ellipsis'}}>
        {lastName}
      </div>
    </div>
  );
}

function Pitch({ players, positions, selectedId, onMove, onTokenClick }) {
  return (
    <div
      data-pitch="1"
      style={{
        position:'relative',
        aspectRatio:'105/68',
        maxHeight:'100%',
        maxWidth:'100%',
        borderRadius:8,
        overflow:'hidden',
        boxShadow:'0 6px 40px rgba(0,0,0,0.8)',
        flexShrink:0,
      }}
    >
      {/* Grass with stripes */}
      <div style={{
        position:'absolute', inset:0,
        background:'#3a8c2f',
        backgroundImage:'repeating-linear-gradient(90deg, transparent, transparent 7.14%, rgba(0,0,0,0.07) 7.14%, rgba(0,0,0,0.07) 14.28%)',
      }} />

      {/* SVG Lines – horizontal */}
      <svg style={{position:'absolute',inset:0,width:'100%',height:'100%',pointerEvents:'none'}} viewBox="0 0 105 68" preserveAspectRatio="none">
        <rect x="2" y="2" width="101" height="64" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        <line x1="52.5" y1="2" x2="52.5" y2="66" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        <circle cx="52.5" cy="34" r="9.15" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        <circle cx="52.5" cy="34" r="0.6" fill="rgba(255,255,255,0.9)"/>
        {/* Left penalty area */}
        <rect x="2" y="13.84" width="16.5" height="40.32" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        <rect x="2" y="24.84" width="5.5" height="18.32" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        <rect x="0.5" y="28.5" width="2" height="11" fill="none" stroke="rgba(255,255,255,0.55)" strokeWidth="0.5"/>
        <circle cx="13.84" cy="34" r="0.6" fill="rgba(255,255,255,0.9)"/>
        <path d="M18.5 26.5 A9.15 9.15 0 0 0 18.5 41.5" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        {/* Right penalty area */}
        <rect x="86.5" y="13.84" width="16.5" height="40.32" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        <rect x="97" y="24.84" width="5.5" height="18.32" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        <rect x="102.5" y="28.5" width="2" height="11" fill="none" stroke="rgba(255,255,255,0.55)" strokeWidth="0.5"/>
        <circle cx="91.16" cy="34" r="0.6" fill="rgba(255,255,255,0.9)"/>
        <path d="M86.5 26.5 A9.15 9.15 0 0 1 86.5 41.5" fill="none" stroke="rgba(255,255,255,0.75)" strokeWidth="0.6"/>
        {/* Corner arcs */}
        <path d="M2 4.5 A2.5 2.5 0 0 1 4.5 2" fill="none" stroke="rgba(255,255,255,0.6)" strokeWidth="0.6"/>
        <path d="M100.5 2 A2.5 2.5 0 0 1 103 4.5" fill="none" stroke="rgba(255,255,255,0.6)" strokeWidth="0.6"/>
        <path d="M103 63.5 A2.5 2.5 0 0 1 100.5 66" fill="none" stroke="rgba(255,255,255,0.6)" strokeWidth="0.6"/>
        <path d="M4.5 66 A2.5 2.5 0 0 1 2 63.5" fill="none" stroke="rgba(255,255,255,0.6)" strokeWidth="0.6"/>
      </svg>

      {/* Tokens */}
      {players.map(p => {
        const pos = positions[p.id];
        if (!pos) return null;
        return (
          <Token
            key={p.id}
            player={p}
            pos={pos}
            selected={selectedId === p.id}
            onDragEnd={onMove}
            onClick={onTokenClick}
          />
        );
      })}
    </div>
  );
}

export default function TaktikBoard() {
  const [team, setTeam] = useState('u17');
  const [formation, setFormation] = useState('4-3-3');
  const [positions, setPositions] = useState({});
  const [selectedId, setSelectedId] = useState(null);
  const [detailPlayer, setDetailPlayer] = useState(null);
  const [sideTab, setSideTab] = useState('squad');

  const buildPositions = useCallback((f, t) => {
    const coords = FORMATIONS[f];
    const squad = PLAYERS[t].filter(p => !p.bench);
    const pos = {};
    squad.forEach((p, i) => { if (coords[i]) pos[p.id] = { x: coords[i][0], y: coords[i][1] }; });
    return pos;
  }, []);

  useEffect(() => {
    setPositions(buildPositions(formation, team));
    setSelectedId(null);
  }, []);

  const applyFormation = (f) => {
    setFormation(f);
    setPositions(buildPositions(f, team));
    setSelectedId(null);
  };

  const switchTeam = (t) => {
    setTeam(t);
    setPositions(buildPositions(formation, t));
    setSelectedId(null);
    setDetailPlayer(null);
  };

  const handleMove = useCallback((id, x, y) => {
    setPositions(prev => ({ ...prev, [id]: { x, y } }));
  }, []);

  const handleTokenClick = useCallback((id) => {
    setSelectedId(id);
    const p = [...PLAYERS.u17, ...PLAYERS.u15].find(x => x.id === id);
    setDetailPlayer(p);
    setSideTab('squad');
  }, []);

  const squad = PLAYERS[team].filter(p => !p.bench);
  const bench = PLAYERS[team].filter(p => p.bench);
  const fKeys = Object.keys(FORMATIONS);

  const tabStyle = (active) => ({
    flex:1, background:'none', border:'none', cursor:'pointer',
    padding:'10px 8px',
    fontFamily:'Barlow Condensed, sans-serif', fontSize:13, fontWeight:700,
    color: active ? '#4aba5e' : '#7a9a7d',
    letterSpacing:'0.5px',
    borderBottom: active ? '2px solid #4aba5e' : '2px solid transparent',
  });

  const fBtnStyle = (active) => ({
    background: active ? '#2d8a3e' : '#181f18',
    border: active ? '1px solid #2d8a3e' : '1px solid rgba(255,255,255,0.08)',
    color: active ? '#fff' : '#7a9a7d',
    fontFamily:'Barlow Condensed, sans-serif', fontSize:13, fontWeight:700,
    padding:'5px 11px', borderRadius:6, cursor:'pointer', whiteSpace:'nowrap',
  });

  return (
    <div style={{ background:'#0c0f0c', color:'#eef3ee', fontFamily:'Barlow, sans-serif', height:'100vh', display:'flex', flexDirection:'column', overflow:'hidden' }}>

      {/* HEADER */}
      <div style={{ background:'#131813', borderBottom:'1px solid rgba(255,255,255,0.08)', padding:'10px 16px', display:'flex', alignItems:'center', justifyContent:'space-between', flexShrink:0 }}>
        <div style={{display:'flex',alignItems:'center',gap:8}}>
          <div style={{width:34,height:34,borderRadius:8,background:'#2d8a3e',display:'flex',alignItems:'center',justifyContent:'center',fontSize:18}}>⚽</div>
          <div>
            <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:20,fontWeight:800,letterSpacing:1,lineHeight:1}}>
              TAKTIK <span style={{color:'#4aba5e'}}>BOARD</span>
            </div>
            <div style={{fontSize:10,color:'#7a9a7d',letterSpacing:'0.5px',marginTop:1}}>FC JUNIOREN</div>
          </div>
        </div>
        <div style={{display:'flex',gap:8,alignItems:'center'}}>
          <select value={team} onChange={e=>switchTeam(e.target.value)} style={{background:'#181f18',border:'1px solid rgba(255,255,255,0.08)',color:'#eef3ee',fontFamily:'Barlow Condensed,sans-serif',fontSize:13,padding:'6px 10px',borderRadius:7,cursor:'pointer'}}>
            <option value="u17">U17</option>
            <option value="u15">U15</option>
          </select>
          <button onClick={()=>applyFormation(formation)} style={{background:'#2d8a3e',border:'1px solid #2d8a3e',color:'#fff',fontFamily:'Barlow Condensed,sans-serif',fontSize:13,fontWeight:600,padding:'6px 12px',borderRadius:7,cursor:'pointer'}}>Reset</button>
        </div>
      </div>

      {/* FORMATION BAR */}
      <div style={{ background:'#131813', borderBottom:'1px solid rgba(255,255,255,0.08)', padding:'8px 16px', display:'flex', alignItems:'center', gap:8, flexShrink:0, overflowX:'auto' }}>
        <span style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:11,fontWeight:700,color:'#7a9a7d',letterSpacing:'1px',textTransform:'uppercase',whiteSpace:'nowrap'}}>Formation:</span>
        {fKeys.map(f => (
          <button key={f} onClick={()=>applyFormation(f)} style={fBtnStyle(formation===f)}>{f}</button>
        ))}
      </div>

      {/* MAIN */}
      <div style={{ flex:1, display:'flex', overflow:'hidden' }}>

        {/* PITCH */}
        <div style={{ flex:1, display:'flex', alignItems:'center', justifyContent:'center', padding:10, background:'#111', overflow:'hidden' }}>
          <Pitch
            players={squad}
            positions={positions}
            selectedId={selectedId}
            onMove={handleMove}
            onTokenClick={handleTokenClick}
          />
        </div>

        {/* SIDEBAR */}
        <div style={{ width:272, background:'#131813', borderLeft:'1px solid rgba(255,255,255,0.08)', display:'flex', flexDirection:'column', overflow:'hidden', flexShrink:0 }}>
          <div style={{display:'flex',borderBottom:'1px solid rgba(255,255,255,0.08)',flexShrink:0}}>
            {['squad','bench','notes'].map((t,i)=>(
              <button key={t} onClick={()=>setSideTab(t)} style={tabStyle(sideTab===t)}>{['Kader','Bank','Notizen'][i]}</button>
            ))}
          </div>

          <div style={{flex:1,overflowY:'auto'}}>
            {sideTab==='squad' && (
              detailPlayer ? (
                <PlayerDetail player={detailPlayer} onBack={()=>{ setDetailPlayer(null); setSelectedId(null); }} />
              ) : (
                squad.map(p=>(
                  <div key={p.id} onClick={()=>handleTokenClick(p.id)} style={{padding:'10px 14px',borderBottom:'1px solid rgba(255,255,255,0.08)',cursor:'pointer',display:'flex',alignItems:'center',gap:10,background:selectedId===p.id?'rgba(45,138,62,0.15)':'transparent',borderLeft:selectedId===p.id?'2px solid #4aba5e':'2px solid transparent'}}>
                    <div style={{width:34,height:34,borderRadius:'50%',background:PG_COLORS[p.pg],display:'flex',alignItems:'center',justifyContent:'center',fontFamily:'Barlow Condensed,sans-serif',fontSize:14,fontWeight:800,color:'#fff',flexShrink:0}}>{p.num}</div>
                    <div style={{flex:1,minWidth:0}}>
                      <div style={{fontSize:13,fontWeight:600,whiteSpace:'nowrap',overflow:'hidden',textOverflow:'ellipsis'}}>{p.name}</div>
                      <div style={{fontSize:11,color:'#7a9a7d',marginTop:1}}>{p.pos} · {p.age}J · {p.foot}</div>
                    </div>
                    <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:16,fontWeight:800,color:ratingColor(p.rating),flexShrink:0}}>{p.rating}</div>
                  </div>
                ))
              )
            )}

            {sideTab==='bench' && (
              <div style={{padding:'10px 14px'}}>
                <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:11,fontWeight:700,color:'#7a9a7d',letterSpacing:'1px',textTransform:'uppercase',marginBottom:8}}>Ersatzbank</div>
                {bench.map(p=>(
                  <div key={p.id} onClick={()=>{ setDetailPlayer(p); setSideTab('squad'); }} style={{padding:'10px 0',borderBottom:'1px solid rgba(255,255,255,0.08)',cursor:'pointer',display:'flex',alignItems:'center',gap:10}}>
                    <div style={{width:34,height:34,borderRadius:'50%',background:PG_COLORS[p.pg],display:'flex',alignItems:'center',justifyContent:'center',fontFamily:'Barlow Condensed,sans-serif',fontSize:14,fontWeight:800,color:'#fff',flexShrink:0}}>{p.num}</div>
                    <div style={{flex:1,minWidth:0}}>
                      <div style={{fontSize:13,fontWeight:600}}>{p.name}</div>
                      <div style={{fontSize:11,color:'#7a9a7d',marginTop:1}}>{p.pos} · {p.age}J</div>
                    </div>
                    <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:16,fontWeight:800,color:ratingColor(p.rating),flexShrink:0}}>{p.rating}</div>
                  </div>
                ))}
              </div>
            )}

            {sideTab==='notes' && (
              <div style={{padding:14}}>
                <div style={{fontFamily:'Barlow Condensed,sans-serif',fontSize:11,fontWeight:700,color:'#7a9a7d',letterSpacing:'1px',textTransform:'uppercase',marginBottom:8}}>Trainer Notizen</div>
                <textarea style={{width:'100%',minHeight:160,background:'#181f18',border:'1px solid rgba(255,255,255,0.08)',borderRadius:8,color:'#eef3ee',fontFamily:'Barlow,sans-serif',fontSize:13,padding:10,resize:'none',outline:'none',lineHeight:1.6}} placeholder="Taktische Hinweise, Anmerkungen…" />
              </div>
            )}
          </div>
        </div>
      </div>
    </div>
  );
}
