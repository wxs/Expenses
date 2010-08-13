Expenses
========

Expenses is a tiny expense tracker written in Python. You use it thus:
    expenses add 3.10 "Cappuccino at Dark Horse"
    expenses plot

Features
--------

- Stores expenses in a very simple CSV file
- Keeps a full version history of expenses in case of user error
- Supports basic reports and plotting of expenses

Why Expenses
------------

If you're like me, you want to keep track of your expenses in a very light-weight fashion. You'll
never track them if you need to wait for a spreadsheet program to open and then nagivate to a particular
cell. Also you have a shortcut for opening the terminal on your computer so a simple command-line interface
is exactly what you need for your expenses.

How do I use Expenses?
----------------

Expenses itself is contained in a single executable. Put that in your PATH somewhere.
It does have the following dependencies:

- Python 2.6+
- Mercurial (This is used to keep your expenses versioned in case you screw them up)
- Matplotlib (If you want to use the plot feature)

When you type "expenses" on the command-line for the first time, a new Expenses setup
is created at `~/.expenses/`. This includes a mercurial repository at `~/.expenses/repo`
which contains your actual expenses file `~/.expenses/repo/expenses.csv`.

You probably won't need to work with that file directly, you can use the `expenses list`
command to view it, and the `expenses edit` command to edit it. By using those commands
you ensure that it stays properly versioned.

Does Expenses work on Windows?
------------------------

No.

Is Expenses exactly the same as PEM?
-----------------------------

They're very similar.

PEM is the [GNU Personal Expense Manager](http://www.gnu.org/software/pem/). It also takes
the minimalist approach and uses a CSV datastore. I wrote this before I knew
that PEM existed, however Expenses has some upsides: its versioning and plotting features do not exist in PEM.
Also I like the pure-python aspect of Expenses.

