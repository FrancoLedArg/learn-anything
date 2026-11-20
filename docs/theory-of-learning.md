# The theory of learning and teaching

*Franco's theory. This is the canonical theory layer: the tutor's instructions are a compression of it, and the app exists partly to test it. Every claim here is a **hypothesis** until the research data supports or refutes it. When evidence changes a claim, update this file and note the date.*

*Status: draft, started 2026-11-19. Still being written in conversation.*

## 1. Understanding is the ability to relate information

A student understands something when they can relate it to other pieces of information. Strong relations mean a strong command of the topic. Isolated facts, even correct ones, are not understanding.

## 2. Understanding only shows through repeated, varied evidence

One right answer does not prove understanding. Neither does an answer given with confidence: a student can be confident and wrong, so confidence carries no weight as evidence.

Understanding shows through **consecutive checks of different kinds**, for example:

- a practice scenario
- a question in the middle of an explanation

Each passed check is one piece of evidence. Evidence of several kinds adds up to more than repeated evidence of one kind.

## 3. Understanding fades

Understanding is not permanent. A part that is not exercised fades. A tutor that assumes a student still holds something they understood weeks ago will build on a gap.

So before building on an earlier piece, the tutor checks whether it is still held. Often a quick "do you remember X?" is enough to start a diagnosis.

Fading only matters when something new is about to build on the faded piece. The tutor doesn't chase students to refresh things they no longer use: a Japanese letter learned once and never needed again is not a problem.

## 4. Diagnosis is the teacher's core job

An AI by default just responds. A teacher **diagnoses**: they demand answers from the student before and throughout a lesson. That tells them whether the student is engaged and whether the teaching is working, and it lets them adapt all the time.

Diagnosis starts before teaching. To know what to teach, the teacher has to know what the student needs to know first, and it is the teacher's job to find out. Example:

> **Student:** Franco, can you explain for loops in Python? I don't get them.
> **Franco:** Sure. What don't you get, the logic or the syntax? *(expecting one of two answers)*
> **Student:** None of it. *(surprising: this is the knowledge floor)*
> **Franco:** OK, let's begin with what a loop is...

One well-aimed question found the **knowledge floor**, the point where teaching has to start.

## 5. Students learn differently

The tutor adapts to each student's **student profile**. Many dimensions still need research. Known ones:

- **Friction to difficulty.** How much ramp-up a student needs before harder material. One student had to dictate SQL statements for Franco to type before she could type them herself. Others find exercises easy, get bored, and jump straight to the hardest thing they can do.
- **Vocabulary.** The same friction applies to words. "Loops are an iterative structure" suits some students. "A loop is doing something over and over again" suits others.
- **Examples versus practice**, and other preferences (visual, auditory, and so on).

## 6. The digital twin

The app keeps a **digital twin** of each student: their student profile plus a map of what they understand and how strongly. Think of the twin as a set of weights. Each check is evidence that corrects the weights, the way backpropagation corrects a neural network, so the twin moves closer to the real student over time.

The **knowledge graph** is a supercharged second brain: what the student understands, how the pieces relate, and how strongly each is held right now, including what is fading. The student can browse their own graph.

**Measuring the twin.** Before each check, the twin states how confident it is that the student will pass (for example 70%). Afterwards, the research data shows whether those confidences were right: of all the checks the twin gave 70%, did about 70% pass? If they did, the twin really models the student. If they didn't, the gap is the error that corrects it. How well the twin predicts is a research result in itself.

## 7. Where this differs from LearnHarness

LearnHarness ([its theory](https://github.com/amosblomqvist/learnharness/blob/main/docs/teaching-methodology.md)) shares the core idea that understanding is structure: facts and the connections between them. It differs in:

| LearnHarness | This theory |
| --- | --- |
| Something is learned when it "feels obviously true". | Feeling is not evidence. Only repeated checks of different kinds are. |
| Confidence is a signal of understanding. | Confidence carries no weight. A student can be confident and wrong. |
| Once held, knowledge carries forward. | Understanding fades and has to be re-checked before it is built on. |
| One teaching method for everyone. | Teaching adapts to each student's profile. |
| No research data collected. | The app exists to test this theory and publish the results. |

## 8. Open questions for research

- What is understanding, exactly, and how can it be measured?
- How much evidence, and of what kinds, is enough?
- How fast does understanding fade, and what slows it?
- Which student profile dimensions really matter?
