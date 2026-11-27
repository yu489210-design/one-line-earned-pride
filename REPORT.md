# REPORT — One Line of Earned Pride

Bounty: https://make.fun/bounty/u-mang-one-line-of-earned-pride-a0138557
Sponsor: Mang (slug `u-mang`). Reward: $5, 10 places (1st $1, 2nd $0.80,
3rd $0.60, 4th $0.50, 5th $0.45, 6th $0.40, 7th $0.35, 8th–10th $0.30).
Entries close 2026-11-27 12:15 Beijing (04:15 UTC). Result due 2026-12-19.
Entry is free. Gate: `/output/entry.txt`, UTF-8, 1–240 characters, not only
whitespace. Field already 4,778 submissions at build time — the final heat
takes the top 500 of the dev board, so the line has to beat the house
anchors, not just be valid.

## Publisher analysis (Mang / u-mang)

Checked 2026-11-27 ~08:20 Beijing, via the make.fun API board
(`GET /api/competitions`, paginated, filtered by sponsor slug `u-mang`):

- Mang has posted exactly 3 bounties, all one-line, all 1–240 characters,
  all house-judged pairwise, all still open — so there are NO finished Mang
  bounties and NO published winning lines to copy from:
  1. One Line of Earned Pride — $5, 4,778 entries, closes 2026-11-27 12:15 Beijing.
  2. The Moon Finally Answers Back — $2, 2,552 entries, closes 2026-11-28.
     "A single line the Moon says back to everyone who has ever stared up
     at it … funny, has to sound like the Moon, lands as a comeback in one read."
  3. The Printer Finally Answers — $2, 2,309 entries, closes 2026-11-29.
     "A single line the office printer would finally say back … funny, has
     to sound like the machine itself, lands its comeback in a single read."
- The sponsor profile page (`/u/u-mang`, `/api/profiles/u-mang`) returns
  404 / "no profile" — Mang is a handle-only sponsor account, no bio or
  history page to read.
- Pattern that can be inferred: every Mang brief is the same shape — one
  line, one voice, one read, judged pairwise by the house brief. The
  "finally answers" pair wants a voice speaking back; this bounty is the
  only one that wants a quiet moment instead of a joke, and its judge brief
  is written by make.fun from the sponsor's request, so the brief itself is
  the best record of what Mang wants.
- How I adjusted: ranked the shortlist by the published judge brief's
  order (earned pride first, then concrete scene, then pride shown not
  told, then one-read landing, then freshness), not by generic funniness.
  Mang's other briefs reward a line that lands in one read with nothing
  left to assemble, so I favoured lines whose last few words do the work
  and cut any line that needed a second read or an explanation.

## Judge brief (from the kit, competition.yaml — read, not guessed)

Judge: z-ai/glm-5.3-flash, pairwise, no ties, two calls per game (both
orders), margin 1–5. Weighs, most important first: (1) genuine earned
pride, a quiet moment, small person doing something hard / long effort
landing — a line off-subject loses to any on-subject line; (2) concrete
scene with a real person, seen happening not summarised; (3) pride earned
inside the line by effort/difficulty the reader can feel, never asserted,
congratulated or explained; (4) lands in one read, pride arrives by the
last word; (5) freshness — not the stock trophy, podium or graduation.
"Plain or funny; only the pride has to be real. Length for its own sake
does not count."

## 25 candidates (all 1–240 chars, counted in Python)

1. (124) The boy split the last log before dark, stacked it straight, and his grandfather nodded once and handed him the axe to keep.
2. (134) After eleven winters, Ana stitched the last square into the quilt, folded it over her grandson's shoulders, and it reached his ankles.
3. (136) At 4 a.m. the baker pulled the first loaf from the oven, tapped its bottom, and heard the hollow knock she'd waited three years to hear.
4. (154) At seventy-one, Mr. Okafor read the bedtime story himself for the first time, and his granddaughter corrected his pronunciation once, then let him finish.
5. (130) Leo read the whole page aloud in class, stuttering only twice, and when he finished he looked up and the room was still listening.
6. (116) After a year of evening classes, he wrote his name in cursive on the form, and the clerk didn't ask him to print it.
7. (120) She played the piece through without stopping for the first time, and her teacher put down his pencil and just listened.
8. (107) She finished the sweater in the hospital waiting room, held it up, and it had both sleeves the same length.
9. (118) He opened the results letter at the kitchen table, read the word pass twice, and folded it into his wallet like money.
10. (123) He sanded the crib until the wood felt like skin, set it beside the bed, and laid his hand flat where the baby would sleep.
11. (139) Rosa finished her last night-school exam at 2 a.m., walked out into the car park, and read the whole bus timetable without moving her lips.
12. (104) Mina held the weld steady for the full seam, lifted her mask, and the bead ran straight as a ruled line.
13. (96) The fisherman mended the last hole in his father's net, cast it at dawn, and it came back heavy.
14. (111) He wrote the letter to his son in English, all by himself, sealed it, and walked it to the mailbox in the rain.
15. (123) She taught her grandmother to video-call, and that evening the old woman rang by herself, held the phone steady, and waved.
16. (133) He laid the last shingle on the roof he'd built with his own hands, climbed down, and stood in the yard looking up at it in the rain.
17. (130) She fixed the puncture with the kit her dad left behind, pumped the tyre hard, and rode past his workshop window without wobbling.
18. (119) Aisha carried the water jug the whole way up the hill without setting it down, and poured the first cup for her mother.
19. (122) She planted the tomato seeds her mother saved, and in August she picked the first red one and ate it standing in the dirt.
20. (120) With his new leg, he danced one slow song with his wife at their daughter's wedding, and didn't sit down until it ended.
21. (120) The janitor buffed the school hall floor until it showed his own face, then stepped back and left his footprints off it.
22. (129) She answered the last question, the officer stamped the paper, and she walked out holding it with both hands like a bowl of soup.
23. (122) The boy signed the whole story to his deaf sister without missing a sign, and she laughed before he reached the punchline.
24. (114) It took her six months, but the dress she'd sewn from her mother's curtains fit, and she wore it to the interview.
25. (132) He practised the speech in the mirror for a month, and when the hall went quiet he said the first line without looking at his notes.

Rejected on first pass: #9 (the "pass" is told, not shown; wallet simile
explains the feeling), #20 (wedding + new leg is two big subjects in one
line; pride is in the dancing, but the setup has to be assembled),
#21 (the floor showing his face is a nice image, but the pride is the
janitor's own reflection — it congratulates itself), #23 (the pride is
really the sister's laughter, not the boy's earned moment), #13 (too
compressed — "came back heavy" lands, but the effort is only implied by
"mended").

## Top 5, pairwise (winner stays)

Shortlist: #1 axe, #2 quilt, #3 baker, #4 bedtime story, #5 stutter.

- #1 vs #2: #1 wins. Both are quiet and concrete, but #2's pride is in a
  measurement ("reached his ankles") while #1's is in a transfer — the
  grandfather giving the axe away. A gift kept beats a size checked.
- #1 vs #3: #1 wins, narrowly. #3 has the best sensory detail (the hollow
  knock) and a three-year wait, but "she'd waited three years to hear" tells
  the reader the wait; #1 shows the wait in "before dark" and "stacked it
  straight" and spends its last words on the handover.
- #1 vs #4: #1 wins. #4 is tender — the granddaughter letting him finish —
  but the earned moment belongs partly to her patience; #1's pride is the
  boy's own, earned by his hands in the line.
- #1 vs #5: #1 wins. #5's last turn ("the room was still listening") is the
  strongest single ending in the set, and the effort (stuttering only
  twice) is felt. But #1's scene is more concrete — a log, a stack, an
  axe, a nod — and its final object (the axe, to keep) is permanent, where
  #5's moment passes when the room moves on.

Winner: #1.

"The boy split the last log before dark, stacked it straight, and his grandfather nodded once and handed him the axe to keep." — 124 characters, one line.

## Submission state

- Entry built directly in this side chat (Muse app session); no subagents.
- `main.py` writes `/output/entry.txt`, run twice, byte-identical
  (sha256 60865d7888baa06d3dcd871fe754576b06ae13e8a655284ff3eacfe0f7f932f4).
- Local commit: a234739ba149ad4ea4bf24cdb97ce47d5ff90c73 (main.py names the
  240-char gate as MAX_CHARS; entry text unchanged).
- Kit check v2 (level-58 kit, bundle transcripts-v2.tar.gz): 14 passed,
  0 failed, 5 skipped, 5 checked at submission (thinking_reproduces 97.6%,
  thinking_revised pass, thinking_priced 1 usage record).
- Bundle: transcripts-v2.tar.gz, 2,388,435 bytes,
  sha256 790dec2eeb4f5ed35fe4b19d19e4b0422190cea0e57465bb159d7f511f9c072a.
  Download: https://muse.ai/files/1346762835195276/29758848983801297/rdblszlhndnqdzu0776f3fdd/transcripts-v2.tar.gz
  (expires 2026-11-29 09:00 Beijing).
- Repo: https://github.com/yu489210-design/one-line-earned-pride (public,
  MIT LICENSE, `.makefun/owner.json` wallet
  6g3axh7HEkjxJwRyi9CDviuxudsRiYF4RxPZoVrK97mH, README badges use
  `yu489210-design/one-line-earned-pride`, About = bounty URL, Topics
  include `makefun`).
- NOT YET SUBMITTED — no submission id, no AI submission. The user submits
  manually in the phone Phantom browser: open the bounty page, fill the
  form (repo + the web HEAD commit + upload the bundle above) and sign in
  Phantom (signature valid 10 minutes, sign at submission time).
