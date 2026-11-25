 # -GaariHub-Pakistani-Car-Marketplace
 /* ===== Part 2 - CSS / Design =====
   All styling: colours, light/dark theme variables, layout, cards, modals, responsive rules.
   Load order in index.html: data.js -> listings.js -> modals.js */
:root{--bg:#f4f6f8;--card:#fff;--tx:#1b2430;--mut:#667085;--pri:#0b6e4f;--acc:#e8a317;--bd:#e2e6ea;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);color-scheme:light}
@media(prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#10151b;--card:#1a212a;--tx:#eef1f4;--mut:#9aa5b1;--pri:#2fb585;--acc:#f0b43a;--bd:#2b3540;color-scheme:dark}}
:root[data-theme="dark"]{--bg:#10151b;--card:#1a212a;--tx:#eef1f4;--mut:#9aa5b1;--pri:#2fb585;--acc:#f0b43a;--bd:#2b3540;color-scheme:dark}
*{box-sizing:border-box}body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;background:var(--bg);color:var(--tx)}
header{background:var(--pri);color:#fff;padding:12px 16px;display:flex;align-items:center;gap:12px;flex-wrap:wrap;position:sticky;top:env(safe-area-inset-top,0px);z-index:5}
header h1{margin:0;font-size:22px}header h1 span{color:var(--acc)}header nav{margin-left:auto;display:flex;gap:8px;flex-wrap:wrap}
button{font:inherit;cursor:pointer;border-radius:8px;border:1px solid var(--bd);background:var(--card);color:var(--tx);padding:8px 14px}
button.p{background:var(--acc);color:#1b2430;border:0;font-weight:700}header button{background:transparent;color:#fff;border-color:#ffffff66}header button.p{border:0;color:#1b2430;background:var(--acc)}
.hero{background:linear-gradient(135deg,var(--pri),#073d2c);color:#fff;padding:28px 16px}.hero h2{margin:0 0 4px;font-size:26px}.hero p{margin:0 0 16px;opacity:.9}
.tabs{display:flex;gap:6px;margin-bottom:10px}.tabs button{background:#ffffff22;color:#fff;border:0}.tabs button.on{background:#fff;color:var(--pri);font-weight:700}
.filters{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:8px;background:var(--card);padding:12px;border-radius:12px;color:var(--tx)}
select,input{font:inherit;padding:9px;border-radius:8px;border:1px solid var(--bd);background:var(--bg);color:var(--tx);width:100%}
main{max-width:1100px;margin:0 auto;padding:16px}.bar{display:flex;justify-content:space-between;align-items:center;gap:8px;flex-wrap:wrap;margin-bottom:12px}.bar select{width:auto}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:14px}
.card{background:var(--card);border:1px solid var(--bd);border-radius:12px;overflow:hidden;cursor:pointer;position:relative}.card:hover{box-shadow:0 4px 16px #0002}
.img{height:130px;display:flex;align-items:center;justify-content:center;font-size:56px}.card .b{padding:12px}.card h3{margin:0 0 4px;font-size:16px}.pr{color:var(--pri);font-weight:800;font-size:18px}.mut{color:var(--mut);font-size:13px}
.tag{position:absolute;top:8px;left:8px;background:var(--acc);color:#1b2430;font-size:11px;font-weight:700;padding:2px 8px;border-radius:99px}
.heart{position:absolute;top:6px;right:6px;border:0;background:#0006;color:#fff;border-radius:50%;width:34px;height:34px;padding:0}.heart.on{color:#ff5c7a}
.empty{text-align:center;color:var(--mut);padding:40px}
.modal{position:fixed;inset:0;background:#000a;display:none;align-items:center;justify-content:center;padding:16px;z-index:20}.modal.show{display:flex}
.box{background:var(--card);border-radius:14px;max-width:520px;width:100%;max-height:90vh;overflow:auto;padding:18px}
.row{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin:8px 0}.box label{font-size:13px;color:var(--mut);display:block}
.spec{display:grid;grid-template-columns:1fr 1fr;gap:6px;margin:10px 0}.spec div{background:var(--bg);padding:8px;border-radius:8px;font-size:14px}
footer{text-align:center;color:var(--mut);padding:24px;font-size:13px}
