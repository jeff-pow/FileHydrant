# Changelog

A history of networks in the file will be kept here.


## **net02** - 4/30/25

### Initial release

- Tune of net01
- Architecture: `(768x9 -> 1536)x2 -> 1`
- 100 SB from 1e-7 to 1e-8 LR with an exponential scheduler
- Weights initialized from a checkpoint from a previous training run, so good luck reproducing this...

```
Elo   | 4.54 +- 2.78 (95%)
SPRT  | 8.0+0.08s Threads=1 Hash=16MB
LLR   | 2.93 (-2.25, 2.89) [0.00, 3.00]
Games | N: 16452 W: 4114 L: 3899 D: 8439
Penta | [59, 1877, 4177, 2016, 97]
https://chess.drpowell.org/test/529/
```

## **net01** - 4/28/25

### Initial release

- First Titan network in an external repository
- Architecture: `(768x9 -> 1536)x2 -> 1`
- 600 SB from 1e-3 to 1e-7 LR with an exponential scheduler
- Weights initialized from a checkpoint from a previous training run, so good luck reproducing this...

```
Elo   | 2.11 +- 1.70 (95%)
SPRT  | N=10000 Threads=1 Hash=16MB
LLR   | 2.89 (-2.25, 2.89) [0.00, 3.00]
Games | N: 100866 W: 38428 L: 37816 D: 24622
Penta | [5593, 9024, 20689, 9432, 5695]
https://chess.drpowell.org/test/520/
```
```
Elo   | 5.16 +- 3.04 (95%)
SPRT  | 8.0+0.08s Threads=1 Hash=16MB
LLR   | 2.90 (-2.25, 2.89) [0.00, 3.00]
Games | N: 14266 W: 3751 L: 3539 D: 6976
Penta | [84, 1583, 3587, 1795, 84]
https://chess.drpowell.org/test/519/
```
