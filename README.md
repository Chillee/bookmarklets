# bookmarklets
Some bookmarklets I find useful

<br>
<a>asdf</a>
<a href="javascript:(function(){const styleSheets = document.styleSheets; let pivotTableRule; for (let i = 0; i < styleSheets.length; i++) { const rules = styleSheets[i].cssRules || styleSheets[i].rules; for (let j = 0; j < rules.length; j++) { if (rules[j].selectorText === '.pivot-table td') { pivotTableRule = rules[j]; break; } } if (pivotTableRule) break; } if (pivotTableRule) { pivotTableRule.style.maxWidth = '1000px'; pivotTableRule.style.overflow = 'hidden'; } else { const style = document.createElement('style'); document.head.appendChild(style); const sheet = style.sheet; sheet.insertRule('.pivot-table td { max-width: 1000px; overflow: hidden; }', 0); }})()"> test </a>
