Repro:

In both A and B package:
- record logs and trace from TSServer in mode verbose
- open index.ts
- create a new files alongside index.ts called foo.ts
- look at the TSServer logs

The TSServer logs of B are longer than the ones of A. It seems like TSServer is recompiling the entire B project when creating a new file but not in A.

