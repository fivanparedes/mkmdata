# MK Mobile Game Data

TSV and TXT files for the RAG system.

## Files

| File | Description | Count |
|------|-------------|-------|
| `characters.tsv` | Character info (name, class, rarity, tier, synergy) | 185 |
| `abilities.tsv` | Special attacks (SP1, SP2, SP3, X-Ray) | 185 |
| `passives.tsv` | Passive abilities | 185 |
| `equipment_basic.tsv` | Basic equipment | 84 |
| `equipment_krypt.tsv` | Krypt equipment | 42 |
| `equipment_towers.tsv` | Tower equipment | 143 |
| `glossary.txt` | Game terminology | ~50 terms |
| `gameplay.txt` | Game mechanics | ~11 sections |

## Adding Data

### Character
1. Add to `characters.tsv`:
   ```tsv
   name	class	rarity	tier	synergy
   New Character	Martial Artist	Diamond	S	Fire damage
   ```

2. Add to `abilities.tsv`:
   ```tsv
   character	sp1	sp2	sp3	xray
   New Character	Fire Punch	Fire Combo		Fatal Blow
   ```

3. Add to `passives.tsv`:
   ```tsv
   character	description
   New Character	Gains 20% attack on fire attack.
   ```

### Equipment
Add to `equipment_basic.tsv` (or appropriate file):
```tsv
name	rarity	type	effect	max_fusion_effect	tier
New Weapon	Epic	Weapon	+20% attack	+50% attack	A
```

## Cache

The `.rag_cache/` folder contains indexed embeddings. Delete it to rebuild:
```bash
rm -rf data/.rag_cache
```
