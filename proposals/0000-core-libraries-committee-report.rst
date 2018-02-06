.. proposal-number:: Leave blank. This will be filled in when the proposal is
                     accepted.

.. highlight:: haskell

Core Libraries Committee Report
==============

Twice a year, the core libraries committee shall produce a plaintext document
specifying which proposals from the libraries mailing list have been accepted
and which have been rejected.

Motivation
----------

The core libraries committee votes on proposals that have been suggested on
the libraries mailing list. Proposals accepted by the committee are allowed
to be implemented the libraries that they oversee. However, the `wiki page`_
for the CLC does not outline how this information is to be diseminated.
The information does not appear to be diseminated through any well-understood
means. The CLC's opinion on proposals fall into one of three categories:

.. _wiki page: https://wiki.haskell.org/Core_Libraries_Committee

* Accepted
* Rejected
* Not Considered

Currently, for the community, the distinction between the Rejected and the
Not Considered categories is difficult to make. For example, consider the
following proposals:

* ordNub: https://mail.haskell.org/pipermail/libraries/2017-October/028269.html
* Data.List.singleton: https://mail.haskell.org/pipermail/libraries/2017-July/028115.html
* Contravariant in base: https://mail.haskell.org/pipermail/libraries/2017-September/028190.html
* Monoid ReaderT: https://mail.haskell.org/pipermail/libraries/2017-November/028312.html

Some of these attracted more discussion than others. Some of them include
comments from members of the CLC. Some of them have only positive responses
and others include mixed reviews. Three of them have shown up multiple
times (from independent authors) on the libraries mailing list in the last
three years. In no case is it clear whether or not the proposal garnered
the CLC's attention or whether it was considered but rejected.

To summarize, there are two problems with the existing system:

* The CLC may inadvertently overlook proposals.
* The community doesn't know whether or not to continue remaking
  old proposals, since it isn't clear whether or not they were
  rejected or overlooked.

Proposed Change
---------------

This proposal suggests a biannual (twice a year) report. The goal is craft this process
in a way that leverages existing infrastructure and community involvement to minimize
the burden that this puts on the CLC.

The report shall be provided by request (more on this later) from the
community on February 1 and August 1 of each year. It shall be headed
with a date range. Proposals from the date range are the ones understood
to be considered in the report. If a proposal made in the date range
is not mentioned in the report, it means that the CLC did not vote on
the proposal. The report shall contain a list of considered proposals
described by the following information:

* Vote: Was the proposal accepted or rejected? The report shall not contain
  an exact breakdown of the votes. Only the result needs to be provided. If
  the committee wish to provide an exact tally to express unanimity or
  significant dissent, they may, but this is not required.
* Name: A brief (no more than ten words) description of the proposal.
* Hyperlink: A link (or multiple links) to the mailing list archive
  where the proposal was originally discussed.

The report does not need to contain an explanation of the decisions made, although
it may include this for particularly difficult decisions if a committee member
wants include it as a note. Here is an example of an August report (based on the
proposals mentioned earlier)::

    Core Libraries Committee August 2018 Report
    Committee votes on proposals from 2018-01-17 to 2018-07-20:

    ACCEPTED, ordNub, https://mail.haskell.org/pipermail/libraries/2017-October/028269.html
    REJECTED, Data.List.singleton: https://mail.haskell.org/pipermail/libraries/2017-July/028115.html
      note: We are willing to reconsider this but want to see broader community support
    ACCEPTED, Contravariant in base: https://mail.haskell.org/pipermail/libraries/2017-September/028190.html
    REJECTED, Monoid ReaderT: https://mail.haskell.org/pipermail/libraries/2017-November/028312.html
    ...

This report would be diseminated through the haskell libraries mailing list.

The responsibility for compiling the list of issues to vote on lies with both
the community and the committee. A lot of what's on the mailing list is
questions and discussions, so filtering through these to find actual
proposals that were met with some level of support (even if it's just
a small amount) is a non-negligible amount of work. A committee member
is permitted (and is encouraged to!) compile the list of issues to be
voted on. If however no report has been released by February 1 or August 1,
any community member may compile the list and request a vote. Clearly,
it would be prudent to inquire on the libraries mailing list to ensure
that another community member (or a CLC member) was not already
working on the list. This will provide a way for the community to
help out if no one on the CLC was get the list together. It will
almost certainly be more likely to reflect the interests of the
individual compiling it, but it's better than not receiving closure
on any of the proposals.

Drawbacks
---------

More work for the CLC. The voting process would likely be impersonal, since
they wouldn't discuss all the issues over a call. I'm not sure if that's
good or bad though.

