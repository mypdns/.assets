# Contribute

If you feel like contributing there are a couple of ways to do this

### Adding a new domain

The workflow is a bit clumsy, but the most reliable and fail-safe.

1. You add an issue with you question, feature request or contribution
   via [Issue templates](https://github.com/mypdns/matrix#issue-templates-quick-links)
   (This is the history of _why_ to blacklist a record)

   ALL fields MOST be filled out, the questions is there for a
   good reason...

2. Add your new domain record(s) to suitable file(s) in the `submit_here/`
   folder.
   An issue is required to be able to historically trace why you
   have committed the records and for other to verify your commit
   without having to visit a pornographic site, for which they actually
   try to avoid by using this list.

3. If you added any content to any of the files in `submit_here/`
   You open an [MR][MR] (Merge Request) where you'll
   add your contribution (This is the _when_ we did the blacklisting)

4. You add the new domain record entry in the top or bottom of the list,
   then it is easier to find.
   The CI/CD code will sort it in alphanumeric order

5. Follow the [New commit](#new-commit) guide

## Manage sub-domain in existing issue domains

Add then in same style and with the usual minimum of need data in a
comment to the primary domain, then if the report is confirmed, it will
be edited into the original issue.

Each individual subdomain should have its own "master" comment.

In that way you can challenge/comment to each subdomain as things will
change over time.

As practised here: https://github.com/mypdns/matrix/issues/201

<details><summary>Click to expand</summary>

![Manage sub-domains]()

</details>

## Why first issue then MR?

The simplest idea is often the most safe, and this is the very reason for this
workflow. It is also giving the project a searchable database for added domains
and the comment, by which we can't add in other ways, as all the lists needs to
be raw data; from which other scripts easily can work with, without first have
to run several cleanup processes.

Please also read
our [Writing Guide](https://kb.mypdns.org/articles/MTX/contributing/Writing-Guide)
before continuing with your issue contribution

# GPG signed

We require all submissions to be signed with a valid GPG key.

Only exception to this rule is the CI/CD bot

## How do I sign with GPG

If you know nothing about GPG keys I, really suggest you search on
[duckduckgo.com][DDG] for the best way, to do it for the OS you
are using.

However, if you do have a GPG key, add it to you submission profile and add a
`-S`
to `git commit -S -m "Some very cool enhancements"` and that is. You can also
set this globally or pr git. Do a search on [duckduckgo.com][DDG]
to figure out the current way.

# Writing files/lines

- All files most end with a newline `\n` (LF) UTF-8.
- All files have to be in universal UTF-8 style without BOM
- Files containing `_windows_` in its filename most be encoded in `ISO-8859-1`
  Latin1 and newlines shall end in (CRLF).
- Line length should not be more than 80 chars for terminals support.

--------------------

# Adult contents contribution

# Contributing

If you feel like contributing there are a couple of ways to do this

1. You can add new super high-speed code, optimizing existing code
   or rewrite for broader support of bash environments across *nix
   OS's

2. You should **_not_** add domains to the `submit_here/` folder of
   this repo. It has to be committed via an ISSUE.

   Because I do have some scripts that handle/maintains several things
   each time an issue is confirmed, like the DNS RPZ zone and the
   repository at once.

# Submit - Contribute

## Workflow

## Add new domains

This one is too simple or therefore probably too good to be
true... right?

Nope, it is true. How can you contribute to 4 Blacklist with
one issue + several RPZ Zone?

1. You open an issue from the list above

   ### Issue comment
   you should know a couple of things about the issue templates,
   as I know a lot of people hates them as I suspect they don't
   understand the long-term and bigger idea behind them.

   Hopefully, the following text might help with that.
    - It is 1 domain = 1 issue
    - The templates are designed so nobody should have to visit any of the
      domains to verify, it is a pornographic domain, hence why the small
      screenshots of the site are required.
    - Everything should, at best, be designed to help others in their goal
      for maintaining and blacklisting adult-related material.
    - We shall always do our best to achieve this so that no one has to
      visit a pornographic site to verify it, once the team behind the
      project has done this.
    - They are designed to match another project (Long term), currently known
      as the matrix, yes because of a $2 domain while watching the matrix
      movie. https://github.com/mypdns/mypdns.org/README.md

2. @spirillen will handle these regularly basis, which usual
   would be a couple of times a week.

**IMPORTANT**: Fill out any fields, or you will at first be requested to
add missing values, if you fail to do this, your commitment can in sever
cases end up being deleted.

## Manage sub-domain in existing issue domains

Add then in the same style and with the usual minimum of need data in a
comment to the primary domain, then if the report is confirmed, it will
be edited into the original issue.

Each subdomain should have its own "master" comment.

In that way, you can challenge/comment to each subdomain as things will
change over time.

As practiced here: https://github.com/mypdns/matrix/issues/201

<details><summary>Click to expand</summary>

![Manage sub-domains]()

</details>

## Screenshot

Why @spirillen is so picky about the screenshots is due to the time
available for him to handle this. You should also have read this
[comment](#issue-comment)

We prefer you upload your fresh screenshot directly to us, as
hot-linking screenshots is bad in most ways, such as 3rd party tracking
and other user data collection and tracking cookies. Minimize the number
of hotlinks used, it's not forbidden as long this won't be abused.
There are also cases where people simply block all 3rd party contents,
they are not able to see any hot-linked contents.

### New code

If you feel like adding new code or modifying existing code to make it run
better, faster, smarter, etc. You will be editing and contributing to the
code, automatically be redirected to a fork of the main repo, from where
you add and/or modify the code.

When you are done with your contribution, you will save the file in
a new branch. Don't forget to make a full reference to the issue in
your commit message as a full URL to issue:

```md
https://github.com/mypdns/matrix/issues<ID>
```

Replace the `<ID>` with the issue id from
https://github.com/mypdns/matrix/issues

![new commit](https://user-images.githubusercontent.com/44526987/134584727-5ce2cc04-6eac-485d-a934-1b730cb1fe44.png)

Next you'll be taken to the `Open a pull request`

![Open a pull request](https://user-images.githubusercontent.com/44526987/134584048-51c583f1-8fe8-4536-831d-8b821077fe57.png)

When everything is filled out correctly, you just hit the
`Create pull request` and you are done.

## GPG signed

We require all submissions to be signed with a valid GPG key.

The only exception to this rule is the CI/CD bot.

### How to sign with GPG

If you know nothing about GPG keys I suggest you search on
[duckduckgo][duckduckgo] for the best way to do it, on your
current OS.

However, if you do have a GPG key, add it to your submission profile add a
`-S` to the `git commit -S -m "Some very cool enhancements"` and that
is. You can set this globally or pr git. Search [duckduckgo][duckduckgo] to
figure out the current way.

### Encoding when writing files/lines

- All files must end with a newline `\n`(LF) UTF-8.
- All files have to be in universal UTF-8 style without BOM
- Any files or file location containing `_windows_` in its files must
  be encoded in `ISO-8859-1 Latin1` and newlines *most* end in (CRLF)
- Line length should not be any longer than 80 chars for supporting
  terminals.

[//]: # Document links

[DDG]: https://duckduckgo.com

[PR]: https://github.com/mypdns/matrix/tree/master/source/porn_filters

[duckduckgo]: https://safe.duckduckgo.com

[akismet]: https://akismet.com/ "Akismet stops spam."


This version supersedes <https://kb.mypdns.org/articles/MTX/Contributing>

Revision date: 28. Nov 2023.

Last edited by: <https://kb.mypdns.org/users/spirillen/>

Approved by: <https://kb.mypdns.org/users/spirillen>

Version: rPD 1.3

[MR]: https://github.com/mypdns/matrix/compare
