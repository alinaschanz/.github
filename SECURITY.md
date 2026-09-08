# security policy

## what these tools do and do not do

everything in my repositories reads public data over public endpoints. none of it holds
keys, signs transactions, or talks to a wallet. the worst a bug can do is print a wrong
number, which is bad enough: people quote numbers.

## reporting

if you find something that makes a tool print a wrong number silently, leak data it should
not (for example an address you passed on the command line ending up in a request to a
third party), or execute anything from a response, please do not open a public issue.
write to **hello@alinaschanz.life** with the repository, the command, and what you saw.
you will get an answer within a few days, a fix as soon as i can, and credit in the release
notes if you want it.

## supported versions

only the latest release of each repository. the tools are small; upgrading is
`pipx upgrade` or a fresh clone.
