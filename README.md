# Hi, I'm Félix-Olivier Dumas

I'm a computer science student from Québec, Canada. I'm mostly interested in **modern C++, compiler engineering, systems programming, and computer architecture**.

<p align="center">
 <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1200&center=true&vCenter=true&width=700&lines=Creator+of+Exotic+CRTP+%26+SPO;Modern+C%2B%2B+%26+Systems+Programming;Template+Metaprogramming;Compiler+Engineering;Concurrency+%26+Memory+Models;SIMD+%26+Vectorization;CPU+Microarchitecture" alt="Typing Animation" />
</p>

My technical interests lie at the intersection of **programming languages, compiler technology, and computer architecture**, with a particular emphasis on understanding how software abstractions translate into machine-level behavior.
   
I work on experimental C++ libraries, language tooling, and LLVM-based compiler infrastructure, exploring **template metaprogramming, compile-time computation, memory management, custom allocators, concurrent data structures, and data-oriented design**. I'm especially interested in zero-overhead abstractions, code generation, and the performance implications of C++ language features. 

A significant part of my independent study and experimentation focuses on **CPU microarchitecture and architecture-aware optimization**, including out-of-order execution, instruction scheduling, branch prediction, cache hierarchies, cache coherence, memory ordering, and **SIMD vectorization**.

I enjoy investigating the relationship between **C++ source code, compiler optimizations, generated assembly, and execution at the microarchitectural level**, particularly where memory access patterns, instruction-level parallelism, and hardware constraints influence performance.

Outside of programming, I'm a classically trained pianist with a particular obsession for Baroque music, especially J. S. Bach. 
 
**[LinkedIn](https://ca.linkedin.com/in/f%C3%A9lix-olivier-dumas-825231394)** · **Discord:** `ferikessu`



<!-- 

Written on November 6, 2026.


Hi there! What brings you here? In all seriousness, if you've landed on this page, you're likely looking to learn a bit more about me. Here's some additional information beyond what's already in the README.

To start, I completed a DEC (college diploma) in Computer Science at Cégep de Rimouski, spanning from the fall of 2023 to the winter of 2026. It was there that I discovered the fundamentals of programming and system design. I spent my days, from morning till night, immersed in design patterns, SOLID principles, and identifying "code smells." This was a pivotal period in my life, as it was when I first discovered my love for programming, though it took a little longer than expected! It wasn't until the summer of 2025 that I began taking an interest in concepts outside of my coursework and experimenting with them. It started with a simple OpenGL project, which served as a great jumping-off point. By the fall of 2025, I truly began to uncover a passion that had been lying dormant within me all along. Specifically, in early October 2025, I first became interested in Data-Oriented Design (DoD) and Entity-Component-System (ECS) architectures. Having started with Java, the language used in my programming classes, I quickly transitioned to C# to explore further.

C# served as the testing ground for my "Apex" project, which is still available in my repositories. Through it, I learned about ECS (Entity-Component-System) design and explored some fundamental concepts related to optimization. Not long after finishing it, I migrated to C++. My goal? To build an ECS that would outperform the one I had refined in C#. As a result, I experimented with templates for the first time! This marked the beginning of something significant, as templates remain my favorite area of focus to this day. This led me to explore C++ further, helping me understand its underlying mechanisms and the ins and outs of the STL (Standard Template Library). I won't list everything here, as my GitHub clearly illustrates my evolution during this period, but suffice it to say that in just a month and a half, I went from understanding `unique_ptr`s to implementing my very first library: Lynx. I also encountered the CRTP (Curiously Recurring Template Pattern) concept, which left a lasting impression on me.

After the Christmas break, I quickly familiarized myself with memory allocators before starting my final semester of college. For this, I had to choose a project to work on independently for two months. I opted to build a comprehensive C++ codebase introspection tool. It was a major, highly complex challenge. It was here that I discovered and experimented with concepts like memory allocation, allocator types, data layout, padding, size optimization, experimental design, and compiler theory. Simply put, the project involved providing the root path of a C++ project so that my tool could analyze every file, generating a complete Abstract Syntax Tree (AST) for each one, capturing the entire C++ language, including functions, members, parameters, types, modifiers, qualifiers, and templates. This metadata was then serialized into JSON (using a custom JSON library I built from scratch). Finally, a code generator would produce a `meta.hpp` file containing the entire code structure, represented through `using` declarations (for types), namespaces, and various "hacks" that allowed for a static representation of the codebase.

The result? You would run my tool and end up with a `meta.hpp` file in your project, allowing you to access introspection data directly within your source code, through paths resembling `meta::classes::Object::functions::foo::parameters::foo::type` or `::name`, for instance. That sort of thing. It was one of the most formative projects I've worked on so far. I might even release it publicly one day, perhaps in a few months or years, once I'm clear of my college's regulations.

This project ran from January 2026 through March. Afterward, I began an internship at my college, which gave me the chance to continue experimenting with C++ on my own. During this time, I was also invited to work on a friend's project: a compiler. I learned a great deal about multithreading, system design, and migrating toward Data-Oriented Design (DoD) or Entity-Component-System (ECS) architectures. I also delved into cache lines, false sharing, spinlocks, and cache locality, concepts I thought I understood, but which turned out to be far more complex than I'd imagined.

The result? I'd work on the compiler with my friend in the evenings, while our days were spent in deep discussions, using whiteboards, iterating on ideas, and so on. It was an incredibly formative experience. This period lasted from mid-March 2026 until early June. I also designed atomic monotonic allocators, a lock-free string interning system, and more. Throughout this process, I kept learning and deepening my knowledge. I spent the entire summer this way, designing systems, having fun, deepening my understanding of compilers, attempting to build one, losing motivation, starting over, all the way up until the beginning of September. I started university and tried to work on a few small projects.

I started with a configuration library based on policy-based design. It's quite niche and a bit of a pain to use, but I'm extremely proud of how the library, and the code itself, looks. That project is called *schematics*. From there, I kept exploring, and suddenly, I decided to learn about SIMD. This served as an introduction to concepts like registers, assembly, standards, and more advanced, low-level techniques. I spent a few days looking into that.

Then, I dove straight into the world of caches: cache lines, spatial locality, internal cache operations, coherence mechanisms, and a much deeper understanding of "false sharing," including the "ping-pong" effect associated with requests for exclusive ownership of cache lines (often illustrated through BusRdX and BusUpgr in simplified coherence models).

Next, I moved on to CPU architecture, specifically out-of-order (OoO) design. I learned about the mechanisms involved in both the front-end and the back-end. For instance, I dissected the BPU (Branch Prediction Unit), including its various subsystems like direction prediction (including classic 2-bit saturating counters) and target prediction (featuring the BTB, etc.). I've been exploring micro-operations, instruction fetching through the iTLB and L1I, the ALU, LSU, ROB, and the op-cache. That's where I am right now.

It's been a little over two weeks since I began studying "mechanical sympathy" (covering everything I just mentioned: caches, SIMD, CPU architecture, etc.), and as of November 6, 2026, just over a year since I started this learning journey, this is where I stand.

I've gone from knowing next to nothing to becoming a respectable developer in the span of a single year. A year is really nothing in the grand scheme of a life, and yet... it's the reason I'm writing this message right now.

I'm not finished yet, far from it. I still have plenty more to share, I assure you. As for where I am right now, I have to admit it feels really great to be here, writing such positive words.

You're probably starting to realize that, while this is technically a "README" file, it's also, and primarily, a letter to my future self. I love sharing, whether it's my personal story or the knowledge I've gained. If this story can inspire you or encourage you to keep going, then I'll consider my mission accomplished.

I'm fully aware that perhaps I shouldn't be laying out my entire life on GitHub like this, but that's just who I am. I can't help it! I look forward to meeting you. Honestly, I'm not even sure why you're still reading this. It's almost suspicious, haha! Anyway, have a great day!

I should point out that this is very condensed. I'm omitting certain significant details, for the obvious reason of keeping the length manageable. I would truly love to include more, but you surely understand that all the words in the world wouldn't be enough to capture the journey that this past year has been!

-->
