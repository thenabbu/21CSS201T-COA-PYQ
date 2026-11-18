# Exam prep strategy for PYQ analysis

**Created:** 11/19/2026 3:06:25  
**Updated:** 11/19/2026 3:11:39  
**Exported:** 11/19/2026 3:16:23  
**Link:** Omitted from the public copy.  

## User:

> 11/19/2026 3:06:26

> File: 21CSS201T-UNIT345-papers-markdown.zip

> File: 21CSS201T-computer-organization-and-architecture.md

okay so

i have

* syllabus md (all 5 units)
* multiple years of pyq papers in md
* unitwise marks composition and sectionwise and questionwise marks composition

issues

* some papers have "slightly" different marking scheme
* some papers have out of syllabus topics /  older syllabus topics
* not all units are coming in the exam

goal

* less study high marks.
* knowing which topics, questions, patterns are reoccuring.
* what to study what not to.
* i am a guy who studies at the end moment, so i want to first study the stuff in such a way so that i can score as much marks as possible with limited time of study.
* what are some hidden patterns and stuff
* what to watch out for
* properly understand the paper and structure

all the data is attachted.

exam marks composition:
unit 3, 4, 5 are coming, marks equaly split among them, total marks 60, 20 units each.

Section A: 12 mcq
section b: 6 questions, 2 per unit, 4 markers, each units set has internal choice for attmepting any 2, or there is per question option among two choices pick any one.
section c: 8 marker questions, with internal choice among two questions attempt any one for that unit, 3 units, 24 marks 

12+24+24=60 marks

## Assistant:

> 11/19/2026 3:11:39

> Comparing the old and new exam formats.
>
> - Checking the saved notes for the exam topic.
> - Updating memory
> - Unzip the PYQ papers and list files with sizes
> - Reading the endsem papers first.
> - Read first three end-sem papers
> - Comparing the old and new exam formats.
> - Read next three end-sem papers
> - Read last two end-sem papers
> - **Done**

Still working through your papers: I've read all 8 end-sem papers and am now reading the internal exams (they're closest to your 3-unit format), then the older-code papers.

> Tallying recurring Unit 1 and 2 questions across the papers.
>
> - Read all internal exam papers (frontmatter stripped)
> - Comparing older course codes with the exam structure.
> - Check which course each older-code paper actually belongs to
> - Listing question text, skipping option lists.
> - Compact dump of 18CSC203J papers (options stripped)
> - Checking which memory topics fall outside the new syllabus.
> - Compact dump of 18CSC003J minors (1-mark Marks lines dropped)
> - Compact dump of 18CSC262J and 19PCSC12T papers
> - Compact dump of 2018 CS0207 and IT0205 papers
> - Tallying recurring Unit 1 and 2 questions across the papers.
> - **Done**

I've now read everything: all 8 end-sems, the 12 internal tests, and the 15 older-code papers. Next I'm running a quick tally so the repeat counts I give you are exact.

> Checking the one-line facts against the earlier papers.
>
> - Tally Part A unit distribution and repeated MCQ stems across 21CSS201T end-sems
> - Rerun tally with fixed index for repeated MCQ stems
> - Tracing which questions in the makeup paper match earlier exams.
> - Find where each recent end-sem question was lifted from earlier papers
> - Checking the one-line facts against the earlier papers.
> - **Done**

I went through all 8 end-sems, the 12 internal tests (CLAT-2, CLAT-3, OBA) and the 15 older-code papers. Your exam boils down to about 5 topics in Unit 3, 3 in Unit 4 and 4 in Unit 5, and the setters recycle heavily.

## How your files map to your format

None of the papers is in your 60-mark, 3-unit format. All 8 end-sems are 75-mark, 5-unit papers (20 MCQs, 8-mark OR-pairs, and a 15-mark OR). So I used these as proxies:

- **Section A:** Part A of the end-sems. About 10–12 of the 20 MCQs per paper come from Units 3–5.
- **Section B (4 marks):** the 4-mark questions in CLAT-2 and CLAT-3, plus Unit 3–5 4-markers from the older codes.
- **Section C (8 marks):** the Q23/Q24/Q25 8-mark OR-pairs for Units 3/4/5.

Three data problems to know about:

- **Unit tags are by topic and sometimes wrong.** De Morgan's, half adders and full adders are Unit 3 in your syllabus, but some papers tag them Unit 1. The 1's/2's-complement subtraction and BCD addition questions are tagged Unit 3 in places, but your syllabus puts them in Unit 1, so they're out.
- **2024 Jul is a typed 130-mark archive copy.** It doesn't match the real format, and the 2023 May file itself says the archive copy doesn't match the scan. Treat it as low-confidence.
- **Older codes have a different syllabus.** Their "Unit 5" is memory, cache and I/O. Only use them for Unit 3–5 topics.

## Hidden pattern 1: the papers are recycled

- **2025 Jul-27 makeup:** 17 of its 20 MCQs are repeats or near-identical rewordings of 2023 May and 2023 Nov. Every Unit 3–5 question in Parts B and C appeared earlier (10÷3 non-restoring, single-bus execution, hazard classes, ARM features, +13×−6 bit-pair, fast adder/CLA).
- **2025 Jul-22:** it was lifted mostly from the internal tests.
  - The fast addition of 11010, 10110, 11011, 10110, 11101, 11111 is from CLAT-2 Set B. The same numbers are also in the OBA and in 18CSC203J Dec 2024.
  - Booth −13×+8 is from CLAT-2 Set B.
  - The unconditional-branch stall is from CLAT-3 Set C.
  - The MUL R2,R3,R4 / ADD R5,R2,R1 hazard is from CLAT-3 Set B.
  - Flynn with example is from CLAT-3 Set C.
  - Its FP add/sub flowchart is near word-for-word from 2023 May.
  - Most of its Unit 3–5 MCQs are also from the CLAT papers.
- **Regular sittings** (May, Nov, Jun) are fresher, but they reuse topics and numbers.

The internal tests are therefore your best question bank, ahead of the older-code papers.

## Hidden pattern 2: the same numbers and instructions come back

- **+13 × −6** appears in 6 papers: 2023 May, 2024 Jul, 2025 Jul-27, CLAT-2 Set D, 18CSC203J 2022 and 19PCSC12T.
- **−13 × +8** appears in CLAT-2 Set B and 2025 Jul-22.
- **−10 × −4** appears in 2023 Nov and CLAT-2 Set C.
- **10 ÷ 3** is non-restoring in 2023 Nov and 2025 Jul-27, and restoring in 4 older papers.
- **Three instructions** cover almost every control-sequence question: `Add (R3),R1` (single bus), `ADD R4,R5,R6` (multiple bus) and `Move (R1),R2`.

## Hidden pattern 3: story problems are standard algorithms

- "Ram and Krishna's multiplier game" is shift-and-add on 13×12.
- "Library racks, 12 books" is non-restoring division, 12÷5.
- "John multiplies −15 and −13 with a flowchart" is Booth.
- "Raghav's mode-control circuit" is the adder/subtractor.
- "Arun and Bob's apples" and "Aravind's marks" are control sequences for an ADD.
- The "weather simulation architect", "project manager" and "security cameras SISD vs SIMD" questions are need for parallelism and Flynn.

## What to study (frequency across the 8 end-sems)

| Unit | Topic | Papers |
|---|---|---|
| 3 | Booth + bit-pair recoding | 7/8 |
| 3 | Fast adder: CLA, carry-save, fast addition | 6/8 |
| 3 | Restoring and non-restoring division | 4/8 |
| 3 | IEEE 754 and FP add/sub flowchart | 4/8 |
| 3 | 4-bit adder/subtractor, full adder | 2/8 |
| 4 | Control sequences (single and multiple bus) | 5/8 |
| 4 | Hazards and remedies, branch handling | 5/8 |
| 4 | Microprogrammed control (diagram, microinstruction format, vs hardwired) | 4/8 |
| 5 | ARM (features, registers and modes, Thumb, load/store, pipeline) | 5/8 |
| 5 | Flynn's classification | 4/8 |
| 5 | Cache coherence / MESI | 4/8 |
| 5 | Need, types and software parallelism | 3/8 |

Counting the 8-mark OR-pairs, the coverage works out like this:

- **Unit 3:** Booth alone would have given you an answerable choice in 7 of 8 pairs.
- **Unit 4:** control sequences plus hazards covers 7 of 8, and adding microprogrammed control covers all 8.
- **Unit 5:** Flynn plus ARM covers only 5 of 8. Adding parallelism types and cache coherence covers all 8.

Cache coherence and MESI aren't in your syllabus text, but they were one of the two options in 4 of 8 papers. Check whether your class notes cover them. If they do, put them in Tier 2 below.

## What to skip

- **Units 1–2:** number systems, gates, complement arithmetic, BCD, Gray code, addressing modes, 8086 and bus structures.
- **Older syllabus:** memory hierarchy, cache mapping and replacement, virtual memory and TLB, ROM/RAM/DRAM, secondary storage, DMA, interrupts, bus arbitration, PCI/SCSI, flip-flops.
- **One-liners only:** RISC vs CISC and UMA/NUMA. They show up as MCQs, not full questions.

## Study order

You're studying at the last minute, so go in this order.

**Tier 1 (most of your marks):**
1. Booth and bit-pair: solve +13×−6, −13×+8 and −10×−4 until you can do them without looking.
2. Non-restoring division on 10÷3 and 14÷5, then restoring on 13÷3.
3. CLA (generate/propagate equations, 4-bit diagram), carry-save addition and the six-number fast-addition problem.
4. IEEE 754 conversions (10.25, 350.2532, −0.75) and the FP add/sub flowchart.
5. The three control sequences above.
6. The hazard types, each with its remedies.
7. The microprogrammed control unit diagram and microinstruction format.
8. Flynn's four classes with examples.
9. ARM features, registers and modes, Thumb and LDR/STR.

**Tier 2:**
- cache coherence and MESI
- pipeline speedup numericals
- the two-state branch-prediction diagram
- hardwired control signal equations (Zin, End)
- memory-mapped vs I/O-mapped I/O (it counts under "basics of I/O operations", and it was a 4-marker twice)
- ILP limitations
- hardware multithreading

**Tier 3:** the MCQ one-liners below.

## Sections A and B

**MCQ one-liners.** Every end-sem had at least one Flynn MCQ.

- Bit-pair recoding halves the summands.
- Booth pair (1,0) → −1.
- The multiplier sits in a shift register.
- IEEE single precision is 1/8/23 bits with bias 127. Double is 1/11/52 with bias 1023. The mantissa is also called the significand.
- The half adder can't take a carry-in. The full adder's carry is XY+XZ+YZ.
- CLA uses generate and propagate.
- NAND = bubbled OR.
- In multiple-bus organisation the registers are called the register file.
- The PC increments by 4 for a 32-bit word.
- WMFC makes the processor wait for memory.
- MAR is the single-directional register.
- A microprogram is the set of microinstructions for one machine instruction.
- Hardwired control is faster but less flexible.
- A data hazard means the operand isn't available. A control hazard is also called an instruction hazard. A structural hazard is hardware contention.
- Software remedy for data hazards is NOPs or compiler reordering. Hardware remedy is operand forwarding.
- A 2-stage pipeline needs 1 buffer and a 4-stage pipeline needs 3.
- Pipelining raises throughput.
- Von Neumann = SISD. Vector processors = SIMD.
- ARM is RISC with a 32-bit core. Thumb is 16-bit and gives smaller code.
- CISC is the complex, expensive one.

**4-mark pool.**
- *Unit 3:* Booth recoding of a given bit-string, CLA generate/propagate numerics, single-precision conversion, shift-and-add on 9×12, full adder from two half adders, the 4-bit adder/subtractor.
- *Unit 4:* roles of control signals (MARin, WMFC, Zin), a short control sequence, hardwired vs microprogrammed, the two-state prediction diagram, the 4-stage pipeline diagram, a pipeline speedup numerical.
- *Unit 5:* Thumb, need and applications of parallelism, ILP, memory-mapped vs I/O-mapped.

**Section B format.** If it's "any 2 from a pool", you can drop your weakest topic. If every question has its own OR, you need shallow breadth across all of the above.

## Watch out for

- **Depth:** the old 12- and 15-mark answers shrink to 8 marks. Aim for a diagram, the steps and one example.
- **Two-part questions** like "(i) advantages of bit-pair, (ii) multiply": the theory half is cheap marks, so don't skip it.
- **Division:** forgetting the final "add M back if A is negative" correction.
- **Booth:** sign errors. Always check the product in decimal.
- **FP:** align exponents, add, normalise, round, then check overflow and underflow.
- **Control sequences:** the standard fetch is PCout, MARin, Read, Select4, Add, Zin; then Zout, PCin, Yin, WMFC; then MDRout, IRin. Learn it as a block.
- **Fresher sittings:** if yours is a regular one, expect some new twists (2025 Jun had 60×40 carry-save and 13÷3 by both methods). The recycling is strongest in makeup sittings.

Want me to turn this into a doc and add worked solutions for the repeated numericals and control sequences?

Powered by Claude Exporter (https://www.ai-chat-exporter.net)
