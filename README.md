# Data Files

TSV files for characters and equipment. TXT files for glossary and gameplay rules.

## Files

| File | Columns | Count |
|------|---------|-------|
| `characters.tsv` | name, class, rarity, tier, synergy | 185 |
| `passives.tsv` | character, description | 185 |
| `abilities.tsv` | character, sp1, sp2, sp3, xray | 185 |
| `equipment_basic.tsv` | name, rarity, type, tier, effect, max_fusion_effect | 84 |
| `equipment_krypt.tsv` | name, rarity, type, tier, effect, max_fusion_effect | 42 |
| `equipment_towers.tsv` | name, rarity, type, tier, effect, max_fusion_effect | 143 |
| `glossary.txt` | Buffs, debuffs, stats definitions | ~50 |
| `gameplay.txt` | Game mechanics and rules | - |

## Tier System

Characters and equipment are ranked:
- **S+** - Exceptionally good / game changer
- **S** - Really good
- **A** - Good
- **B** - Can be useful
- **C** - Not that bad
- **D** - Completely useless

## Cache

RAG embeddings are cached in `.rag_cache/`. Delete to rebuild:

```bash
Remove-Item -Recurse -Force .rag_cache  # Windows
rm -rf .rag_cache                        # Linux/Mac
```
