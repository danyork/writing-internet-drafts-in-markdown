---
title: TODO - Your title
abbrev: TODO - Abbreviation
docname: draft-todo-your-name-here
category: info

ipr: trust200902
area: General
workgroup: TODO Working Group
keyword: Internet-Draft

stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
 -
    ins: T. Todo
    name: Todo Fullname
    organization: TODO Organization
    email: todo@example.com

normative:
  RFC2119:

informative:



--- abstract

This is an example of using markdown in the creation of an Internet Draft. The
specific flavor of markdown being used is kramdown-rfc.

--- middle

# Introduction

TODO Introduction

More infomation can be found in {{?I-D.nottingham-for-the-users}}. (An exmple
of an informative reference to a draft in the middle of text. Note that 
referencing an Internet draft involves replacing "draft-" in the name with 
"I-D.")

# Conventions and Definitions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this
document are to be interpreted as described in BCP 14 {{RFC2119}} {{!RFC8174}}
when, and only when, they appear in all capitals, as shown here.

# Background

This is some background text.

# Use Cases {#usecases}

This section will include some use cases for our new protocol.  The use cases conform
to the guidelines found in {{!RFC7258}}. (Demonstrating a normative 
reference inline.)

Note that the section heading also includes an anchor name that can be referenced in a 
cross reference later in the document, as is done in {{security-considerations}} 
of this document.  (Demonstrating using a reference to a heading without writing an
actual anchor, but rather using the heading name in lowercase and with dashes.)

## First use case

Some text about the first use case. (and an example of using a second level heading.)

HTTP version 2 is defined in {{?HTTP2=RFC7540}}. (Demonstrating renaming a reference so
that it is "HTTP2" instead of "RFC7540". You need to do this the first time you use a
reference. From here on in the document you can just use "HTTP2" in a reference.)

## Second use case

This example includes a list:

- first item
- second item
- third item, with a reference to {{?HTTP2}}.

And text below the list.

# Security Considerations

As outlined earlier in {{usecases}}, there could be security issues in various use
cases.

# IANA Considerations

This document has no IANA actions.



--- back

# Acknowledgments
{:numbered="false"}

Thanks to everyone who helped create the tools that let us use Markdown to create 
Internet Drafts.
