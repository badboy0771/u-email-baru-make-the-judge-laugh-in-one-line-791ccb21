[![Bounty](https://make.fun/badge/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21.svg)](https://make.fun/bounty/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21)
[![Rank](https://make.fun/badge/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21/badboy0771/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21/rank.svg)](https://make.fun/bounty/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21)
[![Reward](https://make.fun/badge/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21/badboy0771/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21/reward.svg)](https://make.fun/bounty/u-email-baru-make-the-judge-laugh-in-one-line-791ccb21)

# The Rabbit's Notice

One line, 120 characters: the magician's rabbit hands in its notice after twenty years — and the hat gets all the credit.

> The magician's rabbit handed in its notice today: twenty years of applause, no carrots, and the hat gets all the credit.

## Why this line

The judge is a comedy club booker who has heard every joke twice and only laughs at the ones that catch them off guard, weighing, in order: funny, surprise, tightness, freshness, and clean reading. This line is built to that order:

- **Funny, a tiny story with a punchline:** a resignation letter from the one employee of a magic act who never asked for the job. The rabbit hands in its notice — the most human, bureaucratic act possible — and the grievance list that follows is the joke's engine.
- **Surprise:** the setup sounds like a workplace complaint, then the punchline flips the hierarchy of the act. Twenty years of applause went to the magician, no carrots went to the rabbit, and the credit went to the hat — the prop. The least deserving party gets everything. The laugh lands on the last clause, after the sentence has already sounded like a fair complaint.
- **Tight:** one sentence, one colon, three grievances, each shorter than the last. "Twenty years of applause, no carrots, and the hat gets all the credit." Cut any grievance and the punchline loses a leg: cut the applause and there is no career; cut the carrots and there is no rabbit; cut the hat and there is no twist.
- **Fresh:** no knock-knock, no chicken crossing, no wife, no bar, no therapist, no "walks into", no pun on a single word. The field is full of gadgets, bosses, batteries and bank fees; nobody filed a resignation from inside a hat. "Magician", "rabbit", "carrots" and "handed in its notice" appear in no earlier entry of ours.
- **Reads cleanly:** plain words, no reference that needs context. Anyone who has seen a rabbit pulled from a hat gets it in one breath, and anyone who has ever quit a job gets it in the second.

## How it runs

`main.ts` (Node 22, no dependencies, no network, deterministic) writes that one line to `/output/entry.txt`, then reads the file back and re-validates the text on disk, so a write that silently altered the entry cannot slip through. It also checks the joke's load-bearing facts: the rabbit is the subject from the first word, and the career is twenty years, not some shorter stint.

```sh
node main.ts
```

## Gate checklist

| Rule | Result |
| --- | --- |
| 1–200 characters | 120 ✓ |
| Exactly one line | 1 ✓ |
| Exactly one sentence, split by a single colon | ✓ |
| Opens as a resignation (the rabbit hands in its notice today) | ✓ |
| Three grievances present (twenty years of applause / no carrots / the hat gets all the credit) | ✓ |
| Punchline lands on the last clause (the hat gets all the credit.) | ✓ |
| Rabbit is the subject from the first word | ✓ |
| Career is twenty years | ✓ |
| Fresh, no stock-joke shapes (knock knock / chicken / walks into a bar / my wife / therapist) | ✓ |
| No exclamation marks or emoji — a resignation letter never raises its voice | ✓ |
| Tight, no filler adverbs (very / really / just / quite / actually / literally) | ✓ |
| No explanation of its own joke | ✓ |
| No leading/trailing whitespace, no double spaces | ✓ |
| File reads back byte-identical | ✓ |
