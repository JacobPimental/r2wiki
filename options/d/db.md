<!-- TITLE: db -->

#  **`db[?]`** Breakpoints commands

Usage: db # Breakpoints commands

- **`db`** List breakpoints
- **`db sym.main`** Add breakpoint into sym.main
- **`db <addr>`** Add breakpoint
- **`db -<addr>`** Remove breakpoint
- **`db.`** Show breakpoint info in current offset
- **`dbj`** List breakpoints in JSON format
- **`dbc <addr> <cmd>`** Run command when breakpoint is hit
  - > Use this to run a command everytime a breakpoint hits. Example: `db sym.imp.strcmp; dbc sym.imp.strcmp drr` . This till print out the registers everytime the debugger breaks at strcmp
  - Screenshot

    ![Dbc](/uploads/small-d/dbc.png "Dbc")

- **`dbC <addr> <cmd>`** Set breakpoint condition on command
- **`dbd <addr>`** Disable breakpoint
- **`dbe <addr>`** Enable breakpoint
- **`dbs <addr>`** Toggle breakpoint
- **`dbf`** Put a breakpoint into every no-return function
- **`dbt[?]`** Display backtrace based on dbg.btdepth and dbg.btalgo
- **`dbt*`** Display backtrace in flags
- **`dbt=`** Display backtrace in one line (see dbt=s and dbt=b for sp or bp)
- **`dbtj`** Display backtrace in JSON
- **`dbta`** Display ascii-art representation of the stack backtrace
- **`dbtv`** Display backtrace with local vars if any
- **`dbte <addr>`** Enable Breakpoint Trace
- **`dbtd <addr>`** Disable Breakpoint Trace
- **`dbts <addr>`** Swap Breakpoint Trace
- **`dbm <module> <offset>`** Add a breakpoint at an offset from a module's base
- **`dbn [<name>]`** Show or set name for current breakpoint
- **`dbi`** List breakpoint indexes
- **`dbic <index> <cmd>`** Run command at breakpoint index
- **`dbie <index>`** Enable breakpoint by index
- **`dbid <index>`** Disable breakpoint by index
- **`dbis <index>`** Swap Nth breakpoint
- **`dbite <index>`** Enable breakpoint Trace by index
- **`dbitd <index>`** Disable breakpoint Trace by index
- **`dbits <index>`** Swap Nth breakpoint trace
- **`dbh x86`** Set/list breakpoint plugin handlers
- **`dbh- <name>`** Remove breakpoint plugin handler
- **`dbw <addr> <rw>`** Add watchpoint
- **`drx number addr len rwx`** Modify hardware breakpoint
- **`drx-number`** Clear hardware breakpoint