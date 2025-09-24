README (as requested, printed here—not inside the ZIP)

Title: Erlang for Beginners — Code Extract
Source: Your uploaded DOCX (chapter-grouped) 

Erlang for Beginners


Generated: Today

What’s inside

A folder per chapter, named Chapter_XX_<title>.

Files are either:

.erl when a module was detected (e.g., -module(...)., -export([...])., -> in function bodies).

.shell.txt for Erlang shell transcripts (lines like 1> ...).

.cli.txt for terminal commands (erl, erlc, rebar3, etc.).

.txt for code-adjacent blocks that don’t clearly fall into the above.

If the book specified a filename via a header like %% File: src/greeter.erl or a trailing hint like src/echo_line.erl:, I used that name. Otherwise, snippets are named snippet_N.ext in the order they appeared.

How I detected and grouped code

Grouped under the most recent “Chapter X …” heading.

Detected code via:

Paragraph style hints (code/monospace where present).

Fixed-width fonts in runs (Courier/Consolas/etc).

Content cues: -module(, -export(, ->, io:, lists:, maps:, case ... of, Erlang shell prompts 1> , and CLI (erl, erlc, rebar3).

Consecutive code paragraphs were merged into a single snippet to avoid splitting one example into many tiny files.

What to expect

Erlang modules: most complete examples like hello.erl, greeter.erl, echo_line.erl, add2.erl, counter.erl, etc., are saved as .erl.

Shell sessions: REPL demos are preserved as .shell.txt for reference.

CLI blocks: build/run commands with erlc or rebar3 live in .cli.txt.

Duplicates: If the same module appears multiple times (e.g., earlier and refined later), both versions are saved; rename or merge as you like before compiling.

How to use the files

For single files:

Open a terminal in the chapter folder.

Compile with erlc filename.erl, then run erl and call module:function(...).

For small “project-style” layouts the book shows:

Create src/ and ebin/ as needed.

erlc -o ebin src/<module>.erl

erl -pa ebin then call functions.

With rebar3 examples:

Use the rebar3 commands in the .cli.txt files.

Limitations and edge cases

DOCX formatting can hide code intent. I used best-effort heuristics. A few non-code lines with arrows -> might be included, and a few plain-paragraph code lines may be missed.

If the book printed two versions of the same module, both are included; compile the one you want.

Shell transcripts aren’t runnable as-is; they’re there to show expected sessions.

Want tweaks?

Prefer separate folders for “examples” vs “exercises”?
I can split by section keywords.

Want only .erl modules zipped, excluding shell/CLI text?
I can regenerate a lean ZIP.

Need a master INDEX.md with per-file descriptions and where they appear in the chapters?
I can produce that too.
