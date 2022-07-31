# DockYard Academy

The DockYard Academy curriculum is an open source curriculum to help students learn Elixir.
The `beta_curriculum` is a work in progress effort available for feedback and contribution.
When launched, this curriculum will be used as the primary teaching material in [DockYard Academy](https://dockyard.com/blog/2022/07/26/what-to-expect-from-the-dockyard-academy-q-a-with-instructor-brooklin-myers).

Contact Brooklin (brooklin.myers@dockyard.com) or DM at [@BrooklinJMyers](https://twitter.com/BrooklinJMyers) on Twitter if you would like more information.

## Want To Get Involved?

Contributors and beta testers are welcome to go through the course, raise issues, and make PRs. See the [Contributor Guide](https://github.com/DockYard-Academy/beta_curriculum/wiki/Beta-Tester-Guide-&-Contributor-Setup).

See our list of [Open Issues](https://github.com/DockYard-Academy/beta_curriculum/issues). Comment on any issue and mention @brooklinjazz to get support.

## QuickStart

1. Clone the project `git clone <URL>`.

2. Install a compatible Elixir and Erlang version. See [.tool-versions](https://github.com/DockYard-Academy/beta_curriculum/blob/main/.tool-versions). You may wish to use [asdf](https://asdf-vm.com/guide/getting-started.html#_1-install-dependencies).

3. Install [Livebook](https://github.com/livebook-dev/livebook):

   ```sh
   mix escript.install github livebook-dev/livebook
   ```
   
4. If using [asdf](https://asdf-vm.com/guide/getting-started.html#_1-install-dependencies) you need to create the [shim](https://github.com/asdf-vm/asdf-elixir#elixir-escripts-support) for livebook.

   ```sh
   asdf reshim
   ```

5. From the project folder run the command below. This opens the navigation
   page where you can find the course reading material and associated
   exercises.

   ```sh
   livebook server start.livemd
   ```

If you cannot see [mermaid.js](https://github.com/mermaid-js/mermaid) graphs,
ensure your Livebook version is correct.

## Troubleshooting

Raise an issue or contact brooklin.myers@dockyard.com if you are having trouble setting up the curriculum.

### LiveBook Desktop App (Currently) Not Supported

Unfortunately, the curriculum is intended to be run from the command line in the project folder. If you're using the livebook desktop app, livebook files will fail to correctly install dependencies. We're working on a fix as soon as possible!

For now, there is a workaround by running livebook with the **Mix standalone** runtime connected to the `utils` project.

To run the project in **Mix Standalone** mode:
1. start livebook.
2. open the curriculum folder in livebook.
3. open `start.livemd` or any other `.livemd` file in livebook.
4. Go to **Runtime Settings**.
5. Click the gear icon.
6. Select **Mix standalone**.
7. Select the `utils` project in the curriculum folder.
8. Click **Connect**.

You should be able to use the curriculum normally now.

Open the curriculum in livebookgo to **Runtime Settings**. 

## Spell Checking

This project uses [codespell](https://github.com/codespell-project/codespell) for spell checking.

If contributing to the project, install codespell and run the following command to fix any spelling errors. Ensure all corrections are correct before committing altered files.

```
codespell --skip="./utils/deps/*,./.git/*,./utils/lib/assets/*" -w
```

## Course Outcome
Students will be competent developers prepared to excel in the Elixir industry. They will have
a solid grasp of Elixir fundamentals, Elixir project development, Phoenix project development, LiveView, and OTP.
They will also have the researching and problem-solving skills necessary to expand their skill set and thrive
throughout their career. Students will be capable of delivering high-quality, well-tested features to a production complexity codebase.

## Curriculum Outline
The curriculum is still a rough outline subject to change and feedback. see [start.livemd](https://github.com/DockYard-Academy/beta_curriculum/blob/main/start.livemd) for a full weekly and daily breakdown.

## Week 1 (Livebook Setup)
1. Course Overview, Command Line, Git, Livebook, PATH
2. Basics (Simple Types, Operators, Variables, Comments)
3. Complex Types (atom, tuples, list, keyword list, map, mapset)
4. Modules, Functions, Structs, Control Flow
5.

## Week 2
1. Problem Solving & Enumeration (ranges, map, filter, all, any, count, find, random)
2. Comprehensions, Enum.reduce
3. Built-In Modules (Map, Tuple, List, Date & Time)
4. Guards, Pattern Matching
5. String Manipulation (Regex, Charlist vs Strings)

## Week 3
1. Polymorphism, Protocols & Behaviors
2. Performance (Immutability, Streams, Lists Vs Tuples Vs Maps Vs Mapsets, Big O, Benchee, :timer) & Recursion
3.
4. File, .iex Scripts, Persistence, Data Validation (Ecto Changesets) (+Binary)
5. Processes (Processes, Generic Server, Genserver, Agents, ETS)

## Week 4 (Dev Setup)
1. Mix Tooling (Credo, Dialyzer, Config, Deps, Documentation, ExUnit)
2. Supervisor Basics and Fault Tolerance (+Task)
3. BEAM
4. Ecto & Database Basics
5.

## Week 5
1. APIs & Parsing JSON
2. Networking Basics & Plug
3. Macros and `use`
4. Deploying Mix Project
5.

## Week 6 (Phoenix Setup)
1. Phoenix Framework & Generators (+ Testing Patterns)
2. HTML & CSS (+ Flex, Grid)
3. Ecto & RDBMS & SQL & Seeding Data
4. Tailwind
5. UX/UI Design + Accessibility (ColorZilla, Axe, Figma)

## Week 7
1. Phoenix Authentication & Permissions
2. LiveView (+ Testing Patterns)
3. JavaScript & JS Interoperability & AlpineJS
4. PubSub & Channels
5. GraphQL & Absinthe (+ Testing Patterns)

## Week 8
1. TDD Techniques (Red Green Refactor), Code Clarity, Mix Testing Tools (--slowest, --stale, tags, Elixir Test extension)
2. Metrics, Telemetry, Live Dashboard
3. Factories & Mocks (ExMachina, Mox)
4. Property Based Testing (Stream Data) + E2E Testing (Wallaby)
5. Code Coverage, Github Actions & Hooks

## Week 9 (Group Project)
1. Software & Product Management (Agile, StandUps, Kanban)
2. Architecture Design & Patterns (Diagrams, UML, CQRS/ES, Contexts, MVC)
3. Advanced Livebook (Graphs, Tables, Connecting Projects)
4. Collaborative GitHub Patterns (PRs, Forking, Cloning, Issues)
5.

## Week 10
1. Emailing & Swoosh
2. Stripe
3. Oban
4. RabbitMQ
5. Kafka

## Week 11
1. Umbrella Projects
2. Genserver Bottlenecks, Supervision Trees, Worker Pools, Tasks
3. Nodes, Clustering
4.
5.


## Week 12 (Final Project)
1.
2.
3.
4.
5.
