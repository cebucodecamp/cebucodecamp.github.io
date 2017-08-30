---
date: 2017-08-29
title: "CTL meets at DNA Micro"
---
## CTL meets at DNA Micro

*Date:* Aug 29, 2017<br />
*Attendees:* Belmer (Host), Murat (Scribe), Froi, Mark

### Discussion of Murat's question: Fairly distributing freedom among a team

Q: How to give team members freedom according to their ability to handle it, while making it fair?

### Discussion of Garik's question: In the zone, how?
Q: What do you do to get into or while you're in the zone?

Answers include: Loud music, white noise, quiet when energy is there and music when energy is needed

### Functional Programming, Talk by Belmer

Summary of points:

• Just a paradigm, like OO
• We do that at DNAμ
• Pure functions, avoid shared state, side-effects, mutation
• There will always be side-effects, but you can separate them out

• Pure function: same input -> same output & no side-effects
• Composition has two solutions:
  1. append function invocations:
    ex: encode(input.split(' ').map(str => str.toLowerCase()).join('-'))
  2. currying, partially bind 
    ex: pipe(split(' '), map(str => str.toLowerCase()), join('-'), encode)
• Shared state: bad because order of function execution changes outcome
• Immutabiility: If you don't share values, then you can't have side-effects. :)
  Trie data structure
• Higher-order functions: Those functions that takes another function as argument
  Allow for advanced composability.
• Declarative vs imperative
  imperative: define how to do something
  declarative: use expressions to define what to do 

• Declarative over imperative
• expressions over statements
• higher order functions over polymorphism

Belmer showed React:
• JSX
• DevTools with its replaying functionality

### Discussion about adding new members

Mark proposed inviting three more people, Garik addad another.
General agreement that it's good to add contributors.
Murat: We're planning a new meetup group for senior coders.

### Discussion of Froi's question: How do you store geo-coordinates?

Belmer: We've just stored plain in MySQL, no querying necessary.
Froi: We'll use Postgres native columns.

### Discussion of self-assessments

Mark proposed one team member during each meeting to do a self-assessment regarding a personal goal or project,
  with others being able to give advice or ask questions.
No consensus, I think.

### Presenting and teaching at school as CTL activity?

Belmer proposed presenting and teaching at schools/universities in Cebu as one of the group's activities.
General agreement it's a good idea. :)
