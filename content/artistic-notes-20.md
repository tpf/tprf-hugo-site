---
title: 'Artistic Notes 2.0'
url: '/artistic-notes-20.html'
---

(The heart of the Artistic license is the idea that
artists, people who create things, should be able to have
ongoing artistic involvement in their work. The goal of the
Artistic 2.0 revision is to make the terms of the original
Artistic License clearer and more readable. In some cases we
expanded it to make it more legally specific. In some cases
we made the language more general so the license may fit
better with past and future changes in technology.

Legal
documents can be considered as just another form of code.
You'll see a lot of spaghetti legal code out there, lengthy
and obtuse, but it doesn't have to be like that. Readability
and maintainability are just as important in legal code as
they are in software. But, because legal documents are code,
our drafting choices are based on a need to capture a
particular legal meaning.

These notes are based
on comments and questions that came up as we worked on this
revision. We hope they will help you understand how to use
the new license. To make the comments easier to follow, we
use Perl as an example in these notes.

### "Original License":

We found ourselves repeating "the version of the
Artistic License that ships with the Standard Version" far
too many times through the license, so we decided to define
it in one place. The "original license" identifies the
license that the developer used to distribute their code. It
also lets the users know that TPRF might update the license
in the future, and that developers who have distributed
under one version of the license can always upgrade to
another. This isn't an automatic upgrade. If you distribute
a package under the Artistic License 2.0, and want to take
advantage of "bug fixes" in version 2.1, you have to include
the new version of the license in the package.

### Section 1:

This section applies to using Perl yourself "as is",
or changing it but only using the changed version yourself
or inside your organization. The rest of the license does
not come into play unless you want to make Perl available to
others, in a standard or modified version.

### Section 2:

You can redistribute unchanged versions of the Perl source
code. You can't charge a licensing fee for it, but you can
charge for distributing it or for providing support.

### Section 3:

Fixing a few bugs, tweaking the code to run on your
operating system, or applying a security patch from the
development mailing list doesn't mean you've created a
"Modified Version".

### Section 4:

You have a few different options if you want to change the
code and redistribute it. Whatever option you choose, you
must let people know that you've changed the code. In
general, we expect that you would do this using a file in
the top-level of the distribution noting what's changed and
that you will update the documentation anywhere your code
works differently from what the documentation says (you
would probably want to do this anyway, so the documentation
isn't misleading). However, there are other ways to meet the
requirements. For instance, you might include a comment in
each changed file, or beside each change in the code.

Under
Section 4(a), you can make any changes you want if you
contribute them back under the Artistic License.

Under
Section 4(b), you can release a proprietary version of the
Perl source code, but if you do, don't pretend your code is
the real Perl. Don't call it Perl, and don't make it so your
users can't use the real Perl on the same machine. This
requirement goes back to the idea of artistic control.

Under
Section 4(c)(i), you can make any changes you want if you
release your changes under the Artistic License.

Section
4(c)(ii) is what we call the "relicensing" clause. Perl 6
(now Raku) and Parrot won't be dual licensed with the GPL,
unlike Perl 5. Since they won't be dual licensed, if you
want to use Perl 6 (now Raku) or Parrot under a GPL license,
you will doing so under 4(c)(ii). Several other open source
and free software licenses also qualify under 4(c)(ii),
including the LGPL, MPL, and the Apache license. Note that
these are only what have become known as "copyleft"
licenses: "freely available" means both free as in speech
and free as in beer.

### Section 5:

If you don't change the code, you can ship it out as
compiled code without the source code. Just tell people how
to get the source code.

### Section 6:

When it comes to Modified Versions, whether you're shipping
compiled code or source code, the requirements are the
same.

### Section 7:

Example: you can ship Perl on a CD along with other
software, or include it in your distribution of Linux.

### Section 8:

You're totally free to embed Perl inside your software in a
way that doesn't allow users to access Perl. On the other
hand, if you embed it and users can nevertheless do things
like running Perl scripts, then you really are distributing
Perl and need make sure that your distribution fits one of
the use cases in (1)-(7).

### Section 9:

When you write code that just runs on Perl, that fact alone
does not make the code subject to the Artistic License. It's
your code. (This seems pretty obvious, but it's important to
say it.)

### Section 10:

The license offers you some rights. In order to obtain
those rights, you need to accept the license. You can reject
the license, but if you do, the rights aren't granted to
you.

### Section 11:

You're responsible for your own actions. If you get a copy
of Perl from someone who broke the terms of the Artistic
License, that doesn't get you off the hook—you're still
required to comply with the license yourself. There are
plenty of places where you can get legal copies of Perl, so
it should be pretty easy to get back into compliance.

### Section 12

:Just being explicit that the license doesn't grant you
trademark rights, or rights related to trademark rights.

### Section 13:

We're not particularly fond of patents, but they're part of
the world we live in. So, with a goal of minimizing the
likelihood of patent infringement claims, we grant you a
patent license. In addition, under our contribution process,
each Contributor makes a patent grant for their
Contributions directly to you as a User. Both patent license
clauses contain a provision that terminates the license(s)
of anyone who files a lawsuit claiming that a Package
infringes any patent. The termination only applies to
Packages that are claimed to be infringements.

### Section 14:

Disclaimers of warranties and damages, like those you find
in other open source and software licenses.

Frequently Asked Questions

### What are the major differences between the Artistic 1.0

and Artistic 2.0?
Overall, the terms of the Artistic 2.0 are the same as
the Artistic 1, though the language has been polished and
reorganized to be more readable and more legally precise.
The significant additions are sections 4(c)(ii) and 13.

### Can I include code from a project licensed under the

GPL in a project licensed under the Artistic license?
No, you can't include code from a GPL (version 1, 2, or 3) project in an Artistic licensed package. Because the
Artistic License (1.0 or 2.0) is a less restrictive
license than GPL (1, 2, or 3). That is, if you distributed
GPL'd code under the Artistic License, you would be giving
away rights that the original author never gave you. The
most obvious example of this is the fact that the Artistic
License allows proprietary versions, but the GPL does
not.

This doesn't prevent you from linking to GPL libraries.
It only prevents you from absorbing GPL code into a
package and distributing that GPL code under an Artistic
License.

### Can I include code from a project licensed under the

Artistic License version 1 in a project licensed under
the Artistic License version 2?
Yes. The terms of Artistic 2.0 are the same as Artistic
1.0, aside from the added patent clause and relicensing
clause. That means Artistic 2.0 is a more restrictive
license than Artistic 1.0 (it gives away fewer rights), so
any Artistic 1.0 code can be distributed as Artistic
2.0.
