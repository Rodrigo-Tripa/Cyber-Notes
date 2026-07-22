# Search Operators

## Overview

Search operators are special commands that refine search engine queries, making it easier to find accurate and relevant information. They are widely used in cybersecurity for researching vulnerabilities, finding documentation, discovering exposed files, and gathering publicly available information (OSINT).

## Exact Match

Use quotation marks to search for an exact phrase.

**Syntax**

```text
"search phrase"
```

**Example**

```text
"Apache HTTP Server 2.4.58"
```

## Search Within a Website

Limit results to a specific domain.

**Syntax**

```text
site:example.com keyword
```

**Example**

```text
site:owasp.org sql injection
```

## Search by File Type

Find specific document formats.

**Syntax**

```text
filetype:pdf keyword
```

**Examples**

```text
filetype:pdf incident response
filetype:ppt cybersecurity
filetype:docx security policy
```

## Exclude Keywords

Remove unwanted results.

**Syntax**

```text
keyword -excluded_word
```

**Example**

```text
python malware -github
```

## Combine Operators

Multiple operators can be used together.

**Example**

```text
site:tryhackme.com filetype:pdf networking
```

This searches only PDF files hosted on the TryHackMe website that contain the word **"networking"**.

## Common Use Cases

Search operators are useful for locating:

- Official documentation
- Technical guides
- Research papers
- Security advisories
- Configuration files
- Publicly available information (OSINT)

## Key Takeaways

- Use `"..."` to search for an exact phrase.
- Use `site:` to limit results to a specific website.
- Use `filetype:` to search for specific document formats.
- Use `-` to exclude unwanted keywords.
- Combine operators to create more precise and efficient searches.