# The Magical Number Seven, Plus or Minus Two (Miller, 1956)

## Citation
- Miller, G. A. (1956). The magical number seven, plus or minus two: Some limits on our capacity for processing information. *Psychological Review*, 63(2), 81–97. https://doi.org/10.1037/h0043158
- Cowan, N. (2001). The magical number 4 in short-term memory: A reconsideration of mental storage capacity. *Behavioral and Brain Sciences*, 24(1), 87–114. (suggests a smaller central capacity, often ~4 chunks)

## Core idea
Miller observed limits in immediate memory and absolute judgment around **7 ± 2** items, and emphasized **chunking**: people can hold more information by grouping elements into meaningful units (chunks). The practical limit is in chunks, not raw bits or characters.

## Key nuances
- Miller himself noted the "seven" coincidence was partly rhetorical; the durable insight is the limit of immediate memory and the power of chunking.
- **Recognition vs. recall**: Miller studied immediate recall/retention. Information that remains visible on screen (menus, lists, labels) is often recognized, not recalled, so it is not constrained the same way as items held in memory. Do not blindly cap visible navigation to 7 items solely because of this paper.
- Later research (e.g., Cowan) suggests the core working-memory capacity may be closer to ~4 chunks in many conditions.

## UX implications (distinct to this principle)
- **Chunk and group related information**: organize content into small, meaningful clusters so it is easier to scan and remember.
- **Structure, don't just shrink**: prefer clear grouping, headings, and whitespace over arbitrary truncation of visible options.
- **Chunk formatted data**: present phone numbers, codes, card numbers, and long identifiers in familiar chunks to aid reading and recall.
- **Limit what must be remembered at once**: when users must carry information across steps (recall), keep the number of items/chunks small (roughly 3–5 to be safe).

## Actionable checks
- [ ] Are related fields, controls, or items grouped into clear, labeled clusters (aim for ~3–5 items per cluster where possible)?
- [ ] Is long numeric/string data chunked into readable segments?
- [ ] If users must remember information between screens/steps, is that memory burden minimized or made visible?
- [ ] Are you using grouping/structure to aid scanning rather than imposing an arbitrary "max 7" limit on visible, recognizable content?
- [ ] Does each cluster have a clear purpose or label?

## External resources
- Original paper (PDF): https://labs.la.utexas.edu/gilden/files/2016/04/MagicNumberSeven-Miller1956.pdf
- Wikipedia — The Magical Number Seven, Plus or Minus Two: https://en.wikipedia.org/wiki/The_Magical_Number_Seven,_Plus_or_Minus_Two
- Laws of UX — Miller’s Law: https://lawsofux.com/millers-law/
- NN/g — Chunking: https://www.nngroup.com/articles/chunking/
